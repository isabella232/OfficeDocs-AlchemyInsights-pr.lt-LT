---
title: Vieno prisijungimo prie "Azure AD" įrenginių trikčių šalinimas
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036174"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Vieno prisijungimo prie "Azure AD" įrenginių trikčių šalinimas

Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie savo skelbimų domeno prijungtuose kompiuteriuose į "Azure AD", galite tai atlikti atlikdami hibridinio "Azure AD" sujungimą. [Kaip: Suplanuokite hibridinį "Azure Active Directory" prisijungti prie diegimo](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) suteikia jums susijusius veiksmus, kad įdiegtumėte hibridinio "Azure AD" sujungimą į aplinką.

Daugiau informacijos ieškokite ["AZURE AD" sujungtų įrenginių konfigūravimas vietiniame Single-Sign "Windows Hello" verslui naudojimas](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos**

Pirminis atnaujinimo žetonas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server" 2016 ir naujesnės versijos, "iOS" ir "Android" įrenginių artefaktas. Tai yra JSON žiniatinklio žetonas (JWT), specialiai išduotas "Microsoft" pirmos šalies simboliniams brokeriams, kad būtų galima įjungti viengubus autentifikacijos (SSO) taikomąsias programas, naudojamas tuose įrenginiuose. Išsamesnės informacijos apie tai, kaip išduodamas PRT, naudojamas ir saugomas "Windows 10" įrenginiuose, rasite [kas yra pirminis atnaujinimo žetonas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: taip ir AzureADPrt: taip**

Šie laukai nurodo, ar vartotojas sėkmingai autentifikuotas "Azure AD" prisijungiant prie įrenginio. Jei reikšmės yra **ne**, taip gali būti dėl:

- Netinkamas saugyklos raktas TPM, susietame su įrenginiu, kai registruojama
- Alternatyvus prisijungimo ID
- Nerastas HTTP tarpinis serveris

Norėdami šalinti įrenginius naudodami komandą dsregcmd, žiūrėkite [SSO būseną](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
