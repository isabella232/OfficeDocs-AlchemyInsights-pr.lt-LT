---
title: 646 Kaip konfigūruoti "AADConnect"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963651"
---
# <a name="configure-sync-features"></a>Sinchronizavimo funkcijų konfigūravimas

"Azure AD Prisijungimas yra kelios funkcijos, kurios įgalintos pagal numatytuosius parametrus arba kurias galite įgalinti vėliau. Kai kurioms funkcijoms reikia papildomos konfigūracijos konkrečiose aplinkose.

- [Filtravimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) riboja objektų sinchronizavimą su "Azure AD". Pagal numatytuosius nustatymus sinchronizuojami visi vartotojai, kontaktai, Windows 10 ir kompiuterio paskyros. Galite įtraukti arba neįtraukti objektų pagal domenus, OUs ar kitus atributus.

- [Slaptažodžių tvarkytuvo sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoja vietinės "Active Directory" slaptažodžių są su "Azure AD". Tai leidžia valdyti slaptažodžius vienoje vietoje, bet naudoti tą patį slaptažodį ir vietinėje, ir debesies aplinkoje. Kadangi "Active Directory" yra patikimas šaltinis, galite naudoti savo slaptažodžių strategijas.

- [Savitarnos slaptažodžio nustatymas iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesyje, tačiau vis tiek taikyti vietinę slaptažodžių strategiją.

- [Įrenginio nurašymas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruotiems "Azure AD" įrenginiams grįžti į vietinę "Active Directory", kad juos būtų galima naudoti sąlyginei prieigai.

- [Pagal numatytuosius nustatymus,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) kad būtų išvengta per daug objektų naikinimo vienu metu (daugiau nei 500 objektų sinchronizavime), įgalinamas atsitiktinis naikinimas. Galite pakeisti šį parametrą, kad jis atitiktų jūsų organizacijos poreikius.

- [Automatinis versijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) naujinimas įjungtas pagal numatytuosius nustatymus skubioms įdiegtims ir padeda užtikrinti, kad jūsų "Azure AD" Prisijungimas visada yra dabartinė.
