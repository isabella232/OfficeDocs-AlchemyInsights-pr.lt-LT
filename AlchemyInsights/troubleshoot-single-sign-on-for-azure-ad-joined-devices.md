---
title: Bendrosios prisijungimo prie "Azure AD" prijungtų įrenginių trikčių šalinimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039254"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Bendrosios prisijungimo prie "Azure AD" prijungtų įrenginių trikčių šalinimas

Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie ad domenu prijungtų kompiuterių prie "Azure AD", tai galite atlikti atlikdami hibridinį "Azure AD" prisijungimą. [Kaip: suplanuokite hibridinę "Azure Active Directory" sujungimo](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) įdiegtį, atlikite susijusius veiksmus, kad jūsų aplinkoje įdiegtų hibridinį "Azure AD" prisijungimą.

Daugiau informacijos žr. "Azure AD" prijungtų įrenginių konfigūravimas [vietiniams įrenginiams Single-Sign On using Windows Hello for Business".](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos**

Pirminis atnaujinimo atpažinimo ženklas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server 2016" ir naujesnėse versijose, "iOS" ir "Android" įrenginiuose artefaktas. Tai JSON žiniatinklio atpažinimo ženklas (JWT), specialiai išduotas "Microsoft" pirmosios šalies atpažinimo ženklų tarpininkams, kad įgalintumėte bendrąją a prisijungimo funkciją (SSO) visuose tuose įrenginiuose naudojamose programose. Išsamios informacijos apie TAI, kaip išleidžiamas, naudojamas ir apsaugotas "Windows 10 įrenginiuose, [žr. Kas yra pirminis atnaujinimo atpažinimo ženklas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES ir AzureADPrt: TAIP**

Šie laukai nurodo, ar vartotojas sėkmingai autentifikavo "Azure AD", kai prisijungia prie įrenginio. Jei reikšmės yra **NE**, taip gali būti dėl:

- Netinkamas saugyklos raktas TPM, susietas su įrenginiu po registracijos (patikrinkite KeySignTest paleisdami padidintą versiją)
- Alternatyvus prisijungimo ID
- HTTP tarpinis serveris nerastas

Norėdami šalinti įrenginių triktis naudodami komandą dsregcmd, žr. [SSO būsena](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
