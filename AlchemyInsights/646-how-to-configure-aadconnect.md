---
title: 646 hvordan du konfigurerer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302722"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunksjoner

Koble til Azure AD inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere. Noen funksjoner krever mer konfigurasjon i bestemte miljøer.
  
- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) grenser objektene synkroniseres Azure AD. Som standard, alle brukere, kontakter, grupper og Windows 10 synkroniseres datamaskinkontoer. Du kan inkludere eller utelate objekter basert på domener, organisasjonsenheter eller andre attributter. 
    
- [Passord hash synkroniseringen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passord hash-koden fra den lokale Active Directory til Azure AD. Dette gjør at passordadministrasjon på ett sted, men bruk av samme passord i både lokale og sky miljøer. Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer for. 
    
- [Self service for å tilbakestille passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) , lar brukerne tilbakestiller sine egne passord i skyen under fortsatt bruk av den lokale policyen. 
    
- [Enheten writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) tillater registrerte enheter i Azure AD skrives tilbake til den lokale Active Directory slik at de kan brukes for betinget tilgang. 
    
- [Forhindre utilsiktet slettinger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktivert som standard for å unngå for mange samtidige objektet slettinger (mer enn 500 objekter per synkronisering). Du kan endre denne innstillingen for å dekke behovene til organisasjonen. 
    
- [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for express installasjoner og bidrar til å sikre din versjon av Azure AD koble alltid er oppdatert. 
    
