---
title: "\"Microsoft Intune\" saugos bazinių linijų naudojimas norint sukonfigūruoti \"Windows 10\" įrenginius"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573537"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>"Microsoft Intune" saugos bazinių linijų naudojimas norint sukonfigūruoti "Windows 10" įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos yra "Windows" parametrų iš anksto sukonfigūruotos grupės, naudojamos, kad būtų taikoma žinoma grupės parametrai ir numatytosios reikšmės, rekomenduojamos atitinkamų saugos komandų. Sukūrę saugos bazinės linijos profilį "Intune", sukuriate šabloną, sudarytą iš kelių įrenginių konfigūracijos profilių.

Kai saugos bazinės linijos diegiamos vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, kurie veikia "Windows 10" arba naujesnę versiją. Pvz., MDM saugos bazinės linijos Automatinis (1) įjungia "BitLocker", skirtą keičiamiesiems diskams (2), reikia slaptažodžio atrakinimo, ir (3) išjungia bazinį autentifikavimą. Kai numatytoji reikšmė neveikia jūsų aplinkoje, tinkinkite bazinę liniją, kad pritaikytumėte norimus parametrus.

Saugumo bazinės linijos taip pat padeda sukurti saugią "Microsoft 365" darbo eigą. Toliau pateikiami keli pranašumai:

- Saugos bazinė linija aprėpia geriausią praktiką ir parametrų, kurie turi įtakos saugai, rekomendacijas. Kadangi "Intune" partneriai su "Windows" saugos komanda, kuri sukuria grupės strategijų bazinių linijų, šios rekomendacijos pagrįstos tvirta rekomendacija ir didelė patirtimi.
- Jei esate naujokas "Intune" ir nežinote, nuo ko pradėti, tada saugos bazinės linijos padės jums greitai sukurti ir įdiegti saugų profilį.
- Jei šiuo metu naudojate grupės strategiją, perėjimas prie Intune valdymo tikslais yra daug lengviau su saugos bazinių linijų, nes jie yra integruoti į Intune ir apima pažangiausius valdymo pajėgumus.

Norėdami sužinoti daugiau, žiūrėkite ["Windows" saugos bazinės linijos](https://go.microsoft.com/fwlink/?linkid=2141503) ir [mobiliųjų įrenginių valdymas](https://go.microsoft.com/fwlink/?linkid=2141701).