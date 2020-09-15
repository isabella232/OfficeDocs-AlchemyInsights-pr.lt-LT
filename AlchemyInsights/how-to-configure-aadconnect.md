---
title: 646 kaip sukonfigūruoti "AADConnect"
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704497"
---
# <a name="configure-sync-features"></a>Sinchronizavimo funkcijų konfigūravimas

"Azure AD Connect" yra kelios funkcijos, kurios įgalintos pagal numatytuosius numatytuosius arba kurias galite įjungti. Kai kurioms funkcijoms reikia papildomos konfigūracijos konkrečiose aplinkose.

- [Filtravimo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limitai objektai sinchronizuojami su "Azure AD". Pagal numatytuosius nustatymą visi vartotojai, kontaktai, grupės ir "Windows 10" kompiuterio abonementai sinchronizuojami. Objektus galite įtraukti arba išskirti pagal domenus, OUs ar kitus atributus.

- [Slaptažodžių maišos sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuojama su "Azure AD" vietinio "Active Directory" slaptažodžių maiša. Tai leidžia valdyti slaptažodį vienoje vietoje, bet naudoti tą patį slaptažodį ir vietinėje, ir debesyje. Kadangi "Active Directory" yra patikimas šaltinis, galite naudoti savo slaptažodžių strategijas.

- [Savitarnos slaptažodžio nustatymas iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesyje, vis dar taikant vietinę slaptažodžių strategiją.

- [Įrenginio įrašymo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) funkcija leidžia registruotiems įrenginiams leisti "Azure AD", kad būtų galima rašyti atgal į vietinį "Active Directory", kad būtų galima naudoti sąlyginę prieigą.

- Kad [atsitiktiniai naikinimai](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) būtų įgalinti pagal numatytuosius nustatymą, kad būtų išvengta per daug vienalaikių objektų naikinimų (daugiau nei 500 objektų sinchronizavime). Galite pakeisti šį parametrą, kad jis atitiktų jūsų organizacijos poreikius.

- [Automatinis versijos naujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) įgalinamas pagal numatytuosius "Express" įrenginiams ir padeda užtikrinti, kad jūsų "Azure AD Connect" versija visada būtų dabartinė.
