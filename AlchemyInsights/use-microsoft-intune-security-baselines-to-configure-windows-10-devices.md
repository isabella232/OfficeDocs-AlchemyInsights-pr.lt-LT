---
title: "\"Microsoft Intune\" saugos bazinių linijų naudojimas norint sukonfigūruoti \"Windows 10\" įrenginius"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696388"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>"Microsoft Intune" saugos bazinių linijų naudojimas konfigūruojant "Windows 10" įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos yra "Windows" parametrų iš anksto sukonfigūruotos grupės, naudojamos, kad būtų taikoma žinoma grupės parametrai ir numatytosios reikšmės, rekomenduojamos atitinkamų saugos komandų. Sukūrę saugos bazinės linijos profilį "Intune", sukuriate šabloną, sudarytą iš kelių įrenginių konfigūracijos profilių.

Kai saugos bazinės linijos diegiamos vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, kurie veikia "Windows 10" arba naujesnėse versijose. Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinės linijos Automatinis (1) įgalina "BitLocker", skirtą keičiamiesiems diskams (2), reikalauja slaptažodžio atrakinimo įrenginio ir (3) išjungia bazinį autentifikavimą. Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytumėte norimus parametrus.

Saugumo bazinės linijos taip pat padeda sukurti saugią "Microsoft 365" darbo eigą. Toliau pateikiami kai kurie šios funkcijos pranašumai:
- Saugos bazinė linija aprėpia geriausią praktiką ir parametrų, kurie turi įtakos saugai, rekomendacijas. Kadangi "Intune" partneriai su "Windows" saugos komanda, kuri sukuria grupės strategijų bazinių linijų, šios rekomendacijos pagrįstos tvirta rekomendacija ir didelė patirtimi.
- Jei esate naujokas "Intune" ir nežinote, nuo ko pradėti, tada saugos bazinės linijos padės jums greitai sukurti ir įdiegti saugų profilį.
- Jei šiuo metu naudojate grupės strategiją, perėjimas prie Intune valdymo tikslais yra daug lengviau su saugos bazinių linijų, nes šios saugos bazinės linijos yra įtaisytos į Intune ir apima pažangiausius valdymo pajėgumus.

Daugiau informacijos ieškokite ["Windows" saugos bazinės linijos](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas](https://docs.microsoft.com/windows/client-management/mdm/).