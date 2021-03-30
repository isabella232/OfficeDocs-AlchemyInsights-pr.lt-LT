---
title: Single-Sign "Azure Active Directory" prijungtiems įrenginiams
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405050"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Vienkartinis prisijungimas prie "Azure Active Directory" prijungtų įrenginių

Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie ad domenu prijungtų kompiuterių prie "Azure AD", tai galite atlikti atlikdami hibridinį "Azure AD" prisijungimą. [Kaip: hibridinio "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sujungimo diegimo planas pateikia susijusius veiksmus, kaip įdiegti hibridinį "Azure AD" prisijungimą jūsų aplinkoje.

["Azure AD" prijungtų įrenginių konfigūravimas vietiniams įrenginiams Single-Sign Naudojant "Windows Hello" verslui](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos** Pirminis atnaujinimo atpažinimo ženklas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server 2016" ir naujesnėse versijose, "iOS" ir "Android" įrenginiuose artefaktas. Tai JSON žiniatinklio atpažinimo ženklas (JWT), specialiai išduotas "Microsoft" pirmosios šalies atpažinimo ženklų tarpininkams, kad įgalintumėte bendrąją a prisijungimo funkciją (SSO) visuose tuose įrenginiuose naudojamose programose. [Dalyje Kas yra pirminis atnaujinimo atpažinimo ženklas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)pateiksime išsamią informaciją, kaip "Windows 10" įrenginiuose išleidžiamas, naudojamas ir apsaugotas PRT.

**WamDefaultSet: YES ir AzureADPrt: TAIP** Šie laukai nurodo, ar vartotojas sėkmingai autentifikavo "Azure AD", kai prisijungia prie įrenginio. Jei reikšmės yra **NE**, gali būti, kad:

- Netinkamas saugyklos raktas TPM, susietas su įrenginiu registruojantis (patikrinkite KeySignTest paleisdami padidintą versiją).
- Alternatyvus prisijungimo ID
- HTTP tarpinis serveris nerastas

Įrenginių trikčių šalinimas naudojant komandą dsregcmd – [SSO būsena](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
