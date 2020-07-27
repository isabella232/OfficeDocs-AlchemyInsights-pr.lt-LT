---
title: Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424219"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune"

Galimybė apeiti aktyvinimo užraktą "iOS" įrenginiuose leidžia lengviau atsigauti pagal scenarijų, kai vartotojas įgalina aktyvinimo užraktą įmonės įrenginyje, o tada palieka įmonę.

Išankstinės aktyvinimo užrakto apėjimo sąlygos:

- Įrenginys yra "prižiūrimas".
- Aktyvinimo užraktas sėkmingai įgalintas naudojant "iOS" įrenginio apribojimo strategiją in Intune.

Be to, apeinant aktyvinimo užraktą turėtumėte:

- Fiziškai turėti prietaisą nušluostyti.
- Nukopijuokite kodą prieš išduokite ištrynimą.

**Pastaba:** Valymo kodas nėra didžiosios ir mažosios raidės, todėl "-" simbolių nereikia.

Daugiau informacijos rasite [Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune".](https://docs.microsoft.com/intune/device-activation-lock-bypass)

**DUK**

Klausimas: **Aš išleido nuotolinio veiksmų pašalinti įmonės duomenis iš įrenginio, ir dabar jis įstrigo laukiančioje būsenoje.**

A: Kad nuotolinis veiksmas būtų sėkmingai užbaigtas, tikslinis įrenginys turi būti internete ir sveikas. Toliau nurodytais atvejais nuotolinis veiksmas lieka laukiančioje būsenoje 30 dienų arba tol, kol įrenginys patvirtina komandą, kai įrenginys:

- Nėra ryšio.
- Praranda savo valdymo statusą su Intune.

Jei manote, kad įrenginys nebeprisiregistruoja ir kad jis nepašalins įmonės duomenų, pasirinkite Naikinti. Panaikinus įrenginio įrašą pašalinamas, kad jis nebebūtų rodomas įrenginių sąraše Intune. Kad įrenginys vėl taptų aktyvus, jo vartotojas turi iš naujo užregistruoti įrenginį.

Klausimas: **Kodėl tam tikrų nuotolinių veiksmų negalima naudoti?**

A: Ne visos platformos palaiko visus nuotolinio įrenginio veiksmus. Šie nuotoliniai veiksmai yra susiję su platforma.

- Apeiti aktyvinimo užraktą (tik "iOS")
- Nauja pradžia (tik "Windows")
- Prarastas režimas (tik "iOS")
- Įrenginio radimas (tik "iOS")
- Paleisti iš naujo (tik "Windows")

Daugiau informacijos apie kiekvieną veiksmą ieškokite [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).