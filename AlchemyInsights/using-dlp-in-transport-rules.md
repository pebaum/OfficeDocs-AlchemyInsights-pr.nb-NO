---
title: Bruker DLP i transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915188"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="cefbd-102">Bruker DLP i transportregler</span><span class="sxs-lookup"><span data-stu-id="cefbd-102">Using DLP in transport rules</span></span>

<span data-ttu-id="cefbd-103">Hvis du vil integrere hindring av tap av data (DLP) i en eksisterende transport, bruker du betingelsen «**Hvis meldingen inneholder...Sensitiv informasjon**» i Transport-regelinnstillingen.</span><span class="sxs-lookup"><span data-stu-id="cefbd-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="cefbd-104">**Hvis du vil ha mer informasjon, kan du se:**</span><span class="sxs-lookup"><span data-stu-id="cefbd-104">**For more details, see:**</span></span>

- <span data-ttu-id="cefbd-105">Integrerte DLP-sensitive informasjonstyper i transportregler: [Integrere sensitive informasjonsregler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="cefbd-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="cefbd-106">Du kan også teste regelen med eller uten policytesting ved hjelp av testmodus på regelen.</span><span class="sxs-lookup"><span data-stu-id="cefbd-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="cefbd-107">Du bør vente 30 minutter etter at du har opprettet regelen før du tester den.</span><span class="sxs-lookup"><span data-stu-id="cefbd-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="cefbd-108">Se [Test e-postflyt/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="cefbd-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="cefbd-109">**Obs**: Hvis du prøver å implementere en ny DLP-policy med transportregler i EAC-en, kan du bruke [DLP-policyer i sikkerhets- og samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.</span><span class="sxs-lookup"><span data-stu-id="cefbd-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>