---
title: Dynamics 365-neteisingas ataskaitų srities rodo Dynamics 365 vieningosios sąsajos
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528559"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Neteisinga ataskaitų srities rodo Dynamics 365 vieningosios sąsajos

Yra kelios priežastys, kodėl galite matyti kitą ataskaitų sritį nei tikitės:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Vartotojas nustatė vartotojo numatytąjį ataskaitų sritį 

Paprastai galite nustatyti vartotojo numatytąją ataskaitų sritį, jei mygtukas **nustatyti kaip numatytąjį** nerodomas ataskaitų srities komandų juostoje. Vartotojo numatytoji ataskaitų sritis pakeis visas kitas numatytąsias ataskaitų sritis, net jei vartotojo numatytoji ataskaitų sritis nėra dabartinėje programėlėje.

Norėdami nustatyti numatytąją ataskaitų sritį, naudokite toliau nurodytą problemos sprendimą.

1. Sukurkite naują asmeninę ataskaitų sritį.

2. Nustatykite naują ataskaitų sritį kaip numatytąją vartotojo.

3. Panaikinkite tą ataskaitų sritį.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Informacijos suvestinė nustatyta svetainės struktūroje

Galite nustatyti organizacijos numatytąjį ataskaitų sritį pasirinkdami ataskaitų sritį ir pasirinkę "nustatyti kaip numatytąjį" dalyje "tinkinti sistemą". Bet informacijos suvestinė, nurodyta svetainės struktūros konstruktoriuje, bus viršesnė už šią ataskaitų sritį, jei vartotojas turi prieigą prie jos.

Jei norite, kad vartotojai matytų ataskaitų sritį, kurią nustatėte kaip numatytąją organizaciją, galite:

* Nustatykite ataskaitų sritį svetainės struktūroje

* Pašalinti prieigą prie svetainės struktūra nustatyta ataskaitų srities tiems vartotojams
