---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250174"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="073f7-102">Problemer med MFA</span><span class="sxs-lookup"><span data-stu-id="073f7-102">Issues with MFA</span></span>
<span data-ttu-id="073f7-103">Det er et par ting du kan kontrollere om brukere ikke kan logge på ved hjelp av multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="073f7-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="073f7-104">Den aktuelle brukeren kan være blokkert i Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="073f7-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="073f7-105">Hvis det er tilfelle, prøver godkjenning for den bestemte brukeren automatisk nektes.</span><span class="sxs-lookup"><span data-stu-id="073f7-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="073f7-106">Følg trinnene i denne artikkelen for å fjerne blokkeringen og dermed.</span><span class="sxs-lookup"><span data-stu-id="073f7-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="073f7-107">Hvis ikke bidra til å deaktivere blokkering av brukeren eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren og de vil gå gjennom prosessen med registrering på nytt.</span><span class="sxs-lookup"><span data-stu-id="073f7-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="073f7-108">Følg trinnene i denne artikkelen.</span><span class="sxs-lookup"><span data-stu-id="073f7-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="073f7-109">Hvis dette er første gangen du aktiverte MFA og brukerne ikke kan logge på ikke-weblesere klienter, for eksempel Outlook, Skype og så videre, er kanskje ADAL (Active Directory-godkjenning Library) ikke aktivert på O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="073f7-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="073f7-110">I dette tilfellet må du koble til Exchange Online Powershell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="073f7-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>