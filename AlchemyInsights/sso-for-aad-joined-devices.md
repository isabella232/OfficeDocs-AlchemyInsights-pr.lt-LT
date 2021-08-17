---
title: Single-Sign įjungtos "Azure Active Directory" įrenginiams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050018"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Prisijungimas prie ""Azure Active Directory" įrenginių

Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie ad domenu prijungtų kompiuterių prie "Azure AD", tai galite atlikti atlikdami hibridinį "Azure AD" prisijungimą. [Kaip: suplanuokite hibridinę "Azure Active Directory" sujungimo](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) įdiegtį, atlikite susijusius veiksmus, kad jūsų aplinkoje įdiegtų hibridinį "Azure AD" prisijungimą.

["Azure AD" prijungtų įrenginių konfigūravimas vietiniame Single-Sign Naudojant "Windows Hello" verslui](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos** Pirminis atnaujinimo atpažinimo ženklas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server 2016" ir naujesnėse versijose, "iOS" ir "Android" įrenginiuose artefaktas. Tai JSON žiniatinklio atpažinimo ženklas (JWT), specialiai išduotas "Microsoft" pirmosios šalies atpažinimo ženklų tarpininkams, kad įgalintumėte bendrąją a prisijungimo funkciją (SSO) visuose tuose įrenginiuose naudojamose programose. [Kas yra pirminis atnaujinimo atpažinimo ženklas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)pateiksime išsamią informaciją apie tai, kaip PRT išleidžiamas, naudojamas ir apsaugotas Windows 10 įrenginiuose.

**WamDefaultSet: YES ir AzureADPrt: TAIP** Šie laukai nurodo, ar vartotojas sėkmingai autentifikavo "Azure AD", kai prisijungia prie įrenginio. Jei reikšmės yra **NE**, gali būti, kad:

- Netinkamas saugyklos raktas TPM, susietas su įrenginiu registruojantis (patikrinkite KeySignTest paleisdami padidintą versiją).
- Alternatyvus prisijungimo ID
- HTTP tarpinis serveris nerastas

Įrenginių trikčių šalinimas naudojant komandą dsregcmd – [SSO būsena](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
