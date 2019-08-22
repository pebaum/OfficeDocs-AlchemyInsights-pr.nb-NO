---
title: Bytt til klassisk rotområdet med et moderne område
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270753"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Bytt til klassisk rotområdet med et moderne område

Hvis miljøet er konfigurert før April 2019, kan du endre rotområdet til et moderne område ved hjelp av Microsoft PowerShell:

- Hvis du har et annet område som du vil bruke som rotområdet, kan du erstatte (swap) primært området med den. 
    - Bruk [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) til å bytte plasseringen av et område med et annet område under arkivering av det opprinnelige området. Tilgjengelig for både Team (ikke koblet til en gruppe) og kommunikasjon-området. 

- Flere muligheter blir introdusert snart som gjør at du kan fortsatt bruke innholdet på området, men du kan konvertere det eksisterende området til et område for kommunikasjon. 
>[!Important]
>Disse funksjonene blir rullet gradvis. Ta en titt på Office 365-Meldingssentral for oppdateringer. 

## <a name="known-issues-with-swapping-sites"></a>Kjente problemer med bytte områder

- Målområdet kan returnere en "not found" (HTTP 404)-feil for en kort tidsperiode.
- Innhold må være kravlesøkt på nytt for å oppdatere søkeindeksen. Det er ingen manuelle trinn nødvendig - dette vil bli gjort automatisk.
- Alt avhengig av "statisk" koblinger (for eksempel filsynkronisering og OneNote-filer) må korrigeres manuelt.
- Hvis kildeområdet var et område for nyheter i organisasjonen, kan du oppdatere URL-adressen.Få en liste over alle organisasjonens nyhetsområder.
- Project Server-områder må kanskje valideres for å sikre at de er fortsatt tilknyttet på riktig måte.




