---
title: 902 (synkroniseringsfeil på grunn av duplisere objekter)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781270"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="d2f3b-102">Synkroniseringsfeil på grunn av duplisere objekter</span><span class="sxs-lookup"><span data-stu-id="d2f3b-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="d2f3b-103">Du kan få en av følgende feilmeldinger når directory-synkronisering er fullført:</span><span class="sxs-lookup"><span data-stu-id="d2f3b-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="d2f3b-104">Kan ikke oppdatere dette objektet i Microsoft Online Services fordi følgende attributter som er knyttet til dette objektet har verdier som allerede er knyttet til et annet objekt i den lokale mappen.</span><span class="sxs-lookup"><span data-stu-id="d2f3b-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="d2f3b-105">En synkronisert objekt med samme proxy-adressen finnes allerede i katalogen for Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="d2f3b-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="d2f3b-106">Kan ikke oppdatere dette objektet fordi følgende attributter som er knyttet til dette objektet har verdier som allerede er knyttet til et annet objekt i lokal mappe-tjenester: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="d2f3b-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="d2f3b-107">For å identifisere og løse problemet, kan du laste ned og kjøre [Verktøyet for IdFix DirSync feil utbedring](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="d2f3b-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="d2f3b-108">Hvis du vil ha mer informasjon, se [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="d2f3b-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  
