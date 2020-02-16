---
title: For fellesmappemigreringsgruppe med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043605"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="efe17-102">For fellesmappemigreringsgruppe med CompletedWithErrors-status</span><span class="sxs-lookup"><span data-stu-id="efe17-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="efe17-103">Bruk følgende fremgangsmåte for å fullføre den satsvise jobben, og hopp over de store/dårlige varene:</span><span class="sxs-lookup"><span data-stu-id="efe17-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="efe17-104">Godkjenne de hoppede varene på migreringsgruppen:</span><span class="sxs-lookup"><span data-stu-id="efe17-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="efe17-105">Set-MigrationBatch \<batchnavn> -ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="efe17-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="efe17-106">Bruk følgende kommando til å godkjenne de hoppede elementene på overføringsforespørsler som er "Synkronisert", men ikke fullført:</span><span class="sxs-lookup"><span data-stu-id="efe17-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="efe17-107">$pf=Få-publicfolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i i $pf) {hvis ($i.LargeItemsEncountered -gt 0 -eller $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="efe17-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="efe17-108">Migreringsgruppen og forespørslene skal gjenopptas og fullføres om noen få minutter.</span><span class="sxs-lookup"><span data-stu-id="efe17-108">The migration batch and requests should resume and complete in a few minutes.</span></span>
