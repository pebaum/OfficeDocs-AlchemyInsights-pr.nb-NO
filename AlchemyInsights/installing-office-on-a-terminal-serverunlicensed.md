---
title: Installere office på en Terminal Server - ulisensiert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303265"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d1ea0-102">Installere Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="d1ea0-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d1ea0-103">For distribusjon av Office 365 ProPlus på en Windows-Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="d1ea0-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d1ea0-p101">Du må ha en Office 365-plan som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5. Office 365 Business og Office 365 Business Premium planene inkluderer ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="d1ea0-106">Du må aktivere [delt datamaskinaktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="d1ea0-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="d1ea0-107">Hvis du vil installere Office 365 ProPlus på RDS fra Office 365-portalen \*\* *som bruker standardinnstillingene for installasjonen* \*\*, følger du denne fremgangsmåten:</span><span class="sxs-lookup"><span data-stu-id="d1ea0-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="d1ea0-p102">Se hva du har Office 365-planen. [Lære hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="d1ea0-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="d1ea0-p103">Hvis nødvendig, bytte til en annen Office 365-planer. [Lære hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="d1ea0-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="d1ea0-p104">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, kan du avinstallere den. For eksempel ved å gå til Kontrollpanel \> Avinstaller et program. Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting-hjelperen](https://aka.ms/SARA-OfficeUninstall-Alchemy) Hvis du kjører i problemer.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="d1ea0-115">Logg på Office 365-portalen med administrator-kontoen og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="d1ea0-116">Etter at Office er installert, \*\* *ikke åpne eller logge deg på* \*\* til alle Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="d1ea0-117">På RDS-server, kan du aktivere delt datamaskinaktivering ved å redigere registret ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="d1ea0-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="d1ea0-p105">Høyreklikk Windows-knappen nederst til venstre på skjermen og velg Kjør. Skriv inn **regedit**i Åpne-boksen, og velg deretter OK.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="d1ea0-120">Velg Ja når du blir bedt om å tillate Registerredigering til å gjøre endringer til enheten.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="d1ea0-121">I Registerredigering, legge til en strengverdi på **SharedComputerLicensing** med innstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d1ea0-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="d1ea0-122">På RDS-server \*\* *Logg på som en sluttbruker* \*\* og [Kontroller at delt datamaskinaktivering er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d1ea0-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="d1ea0-123">Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av verktøyet for distribusjon av Office, kan du se [Distribuere Office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d1ea0-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="d1ea0-124">Hvis du vil rette opp feil i forbindelse med aktivering av delt datamaskin, kan du se [Feilsøke problemer med delt datamaskin aktiveringsveiviseren for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="d1ea0-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
