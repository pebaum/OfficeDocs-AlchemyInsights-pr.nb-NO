---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057748"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="dc516-102">Kan ikke slette elementer</span><span class="sxs-lookup"><span data-stu-id="dc516-102">Unable to delete items</span></span>

<span data-ttu-id="dc516-103">Har du problemer med elementer slettes?</span><span class="sxs-lookup"><span data-stu-id="dc516-103">Having issues deleting items?</span></span>

- <span data-ttu-id="dc516-104">Kontroller alltid at du har [riktige tillatelser](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) til å slette elementet eller har en [administrator for områdesamling](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) forsøk på fjerne elementet.</span><span class="sxs-lookup"><span data-stu-id="dc516-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="dc516-105">Kontroller at det ikke er et oppsett for [oppbevaringspolicy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) på varen.</span><span class="sxs-lookup"><span data-stu-id="dc516-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="dc516-106">Kontroller at elementet ikke er [sjekket ut](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en annen bruker.</span><span class="sxs-lookup"><span data-stu-id="dc516-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="dc516-107">Til slutt, kan administratorer bruke [SharePoint mønstre og praksiser](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som inneholder et bibliotek med PowerShell kommandoer som gjør det mulig å utføre komplekse management handlinger som tvinger sletting av stubborn elementer.</span><span class="sxs-lookup"><span data-stu-id="dc516-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="dc516-108">Fjern PNP-fil</span><span class="sxs-lookup"><span data-stu-id="dc516-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="dc516-109">Fjern PNP-mappe</span><span class="sxs-lookup"><span data-stu-id="dc516-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="dc516-110">Fjern PNP listeelement</span><span class="sxs-lookup"><span data-stu-id="dc516-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="dc516-111">Fjern PNP-listen</span><span class="sxs-lookup"><span data-stu-id="dc516-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="dc516-112">Fjern PNP-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="dc516-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)