---
title: 646 Kaip sukonfigūruoti AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722571"
---
# <a name="configure-sync-features"></a>Sinchronizavimo funkcijų konfigūravimas

"Azure AD Connect" yra kelios funkcijos, kurios įgalintos pagal numatytuosius nustatymus arba kurias galite įgalinti vėliau. Kai kurioms funkcijoms reikia papildomos konfigūracijos konkrečiose aplinkose.

- [Filtravimo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) apribojimai objektai sinchronizuojami su Azure AD. Pagal numatytuosius nustatymus sinchronizuojami visi vartotojai, kontaktai, grupės ir "Windows 10" kompiuterių abonementai. Galite įtraukti arba išskirti objektus pagal domenus, ous ar kitus atributus.

- [Slaptažodžio maišos sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoja slaptažodžio maišą iš vietinės "Active Directory" į "Azure AD". Tai leidžia valdyti slaptažodžius vienoje vietoje, bet naudoti tą patį slaptažodį tiek vietinėje, tiek debesies aplinkoje. Kadangi "Active Directory" yra patikimas šaltinis, galite naudoti savo slaptažodžių strategijas.

- [Savitarnos slaptažodžio nustatymas iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesyje, tačiau vis dar taiko jūsų vietinę slaptažodžio politiką.

- [Įrenginio perrašymas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruotus įrenginius Azure AD galima rašyti atgal į vietinę Active Directory, kad jie gali būti naudojami sąlyginės prieigos.

- [Užkirsti kelią atsitiktiniams naikinimams](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) pagal numatytuosius nustatymus įgalinta, kad būtų išvengta per daug vienu metu esančių objektų naikinimų (daugiau nei 500 objektų sinchronizuojant). Šį parametrą galite pakeisti, kad jis atitiktų jūsų organizacijos poreikius.

- [Automatinis naujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) yra įjungtas pagal numatytuosius nustatymus express įrenginių ir padeda užtikrinti, kad jūsų versija Azure AD Connect visada yra dabartinis.
