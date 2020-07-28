---
title: Prarastų "iOS" įrenginių radimas naudojant "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439630"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Prarastų "iOS" įrenginių radimas naudojant "Intune"

Įjungus prarastą režimą "iOS" įrenginyje, administratorius gali užrakto ekrane rodyti pranešimą ir kontaktinį telefono numerį.

Įjungus prarastą režimą, administratorius gali naudoti veiksmą Rasti įrenginį, kad nustatytų fizinę įrenginio vietą.

"Intune" veiksmas Rasti įrenginį veikia su "iOS" įrenginiais, kad žemėlapyje būtų rodoma konkretaus įrenginio vieta.

Norint atlikti šį veiksmą, reikia, kad "iOS" įrenginys būtų:

- Prižiūrimas režimas
- Prarastas režimas

Daugiau informacijos rasite ["iOS" / "iPadOS" įrenginiuose su "Intune" įjungta prarastu režimu](https://docs.microsoft.com/intune/device-lost-mode) ir [raskite pamestus ar pavogtus "iOS" / "iPadOS" įrenginius su "Intune" įrenginiais.](https://docs.microsoft.com/intune/device-locate)

**DUK**

Klausimas: Aš išleido nuotolinio veiksmų pašalinti įmonės duomenis iš įrenginio, ir dabar jis įstrigo laukiančioje būsenoje.

A: Kad nuotolinis veiksmas būtų sėkmingai užbaigtas, tikslinis įrenginys turi būti internete ir sveikas. Toliau nurodytais atvejais nuotolinis veiksmas lieka laukiančioje būsenoje 30 dienų arba tol, kol įrenginys patvirtina komandą:

- Kai prietaisas neturi ryšio su
- Kai prietaisas praranda valdymo būseną su Intune

Jei manote, kad įrenginys nebeprisiregistruoja ir negalės pašalinti įmonės duomenų, pasirinkite Naikinti. Panaikinus įrenginio įrašą pašalinamas, kad jis nebebūtų rodomas įrenginių sąraše Intune. Jei įrenginys vėl įsijungia, jo vartotojas turės jį užregistruoti iš naujo.

Klausimas: Kodėl tam tikrų nuotolinių veiksmų negalima naudoti?

A: Ne visos platformos palaiko visus nuotolinio įrenginio veiksmus. Šie nuotoliniai veiksmai yra susiję su platforma, todėl jie pasiekiami tik pažymėtiems platformoms.

- Apeiti aktyvinimo užraktą (tik "iOS")
- Nauja pradžia (tik "Windows")
- Prarastas režimas (tik "iOS")
- Įrenginio radimas (tik "iOS")
- Paleisti iš naujo (tik "Windows")

Daugiau informacijos apie kiekvieną veiksmą ieškokite [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).