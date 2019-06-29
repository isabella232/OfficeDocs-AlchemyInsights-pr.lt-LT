---
title: 646 kaip sukonfigūruoti AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385362"
---
# <a name="configure-sync-features"></a>Konfigūruoti sinchronizavimo funkcijos

Žydros AD jungtis yra kelios funkcijos, yra įjungta pagal numatytuosius nustatymus, arba, kad galite įgalinti vėliau. Kai kurios funkcijos reikalauja papildomos konfigūracijos konkrečių aplinkoje.

- [Filtravimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ribas objektai yra sinchronizuoti su Azure AD. Iš numatytasis, visi vartotojai, kontaktus, grupes ir "Windows 10" sinchronizuojami kompiuterių sąskaitos. Jūs galite įtraukti arba pašalinti objektus, domenai, organizaciniai vienetai ar kiti atributai.

- [Slaptažodis maiša sinchronizavimo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoja slaptažodį maišos iš vietinės Active Directory su Azure AD. Tokiu būdu slapta˛od˛io valdymo vienoje vietoje, bet naudoti tą patį slaptažodį, tiek vietiniame ir debesų kompiuterijos aplinkose. Todėl, kad Active Directory yra patikimas šaltinis, galite naudoti savo slaptažodžio strategijų.

- [Savitarnos slaptažodžio nustatymo iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesis dar taikant vietinę slaptažodžių strategija.

- [Įrenginio write-back](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruoti įrenginiai Azure AD įrašomi atgal į vietinės Active Directory, jie gali būti naudojami dėl sąlygine prieiga.

- [Išvengti atsitiktinio panaikina](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) yra įjungta pagal nutylėjimą padeda išvengti per daug vienu metu objektas naikinimus (daugiau kaip 500 objektų už sinchronizavimo). Galite pakeisti šį nustatymą, kad atitiktų jūsų organizacijos poreikius.

- [Automatinis atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) įgalintas pagal numatytuosius nustatymus aiškaus įrenginiams ir padeda užtikrinti jūsų versija Azure AD Connect visada yra dabartinė.
