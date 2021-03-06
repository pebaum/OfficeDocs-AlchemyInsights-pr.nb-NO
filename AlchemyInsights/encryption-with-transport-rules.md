---
title: Kryptering med transportregler
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
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915171"
---
# <a name="encryption-with-transport-rules"></a>Kryptering med transportregler

I [administrasjonssenteret for Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) kan du bruke funksjoner for Office-meldingskryptering (OME) i e-postflytreglene dine for å utløse meldingskryptering. Velg alternativet **Bruk Office 365-meldingskryptering og rettighetsbeskyttelse** i Transportregel-betingelsen.

- Hvis du vil ha mer informasjon, kan du se [Definere regel for postflyt for å kryptere](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- I PowerShell bruker du [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities)-cmdleten og setter *ApplyOME*-parameteren til $true.
