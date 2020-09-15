---
title: Dynamics 365 – neteisinga ataskaitų srities rodoma "Dynamics 365" bendroji sąsaja
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711283"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Neteisinga ataskaitų srities rodoma Dynamics 365 bendroji sąsaja

Yra kelios priežastys, kodėl galite matyti kitokią ataskaitų sritį nei tikitės:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Vartotojas nustatė vartotojo numatytąjį ataskaitų sritį 

Paprastai galite nustatyti vartotojo numatytąjį ataskaitų sritį, jei mygtukas **nustatyti kaip numatytąjį** nerodomas ataskaitų srities komandų juostoje. Vartotojo numatytoji ataskaitų sritis pakeis visas kitas numatytąsias ataskaitų sritis, net jei vartotojo numatytosios ataskaitų srities nėra dabartinėje taikomojoje programoje.

Norėdami panaikinti numatytąjį ataskaitų sritį, naudokite šį sprendimo būdą.

1. Kurti naują asmeninį ataskaitų sritį.

2. Nustatyti naują ataskaitų sritį kaip numatytąjį vartotojo.

3. Naikinti tą ataskaitų sritį.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Ataskaitų sritis nustatyta struktūra

Galbūt nustatėte organizacijos numatytąją ataskaitų sritį pasirinkdami ataskaitų sritį ir pasirinkę "nustatyti kaip numatytąjį" dalyje "tinkinti sistemą". Tačiau, jei vartotojas turi prieigą prie šio ataskaitų srities, pagal šią ataskaitų sritį bus teikiama pirmenybė schemos dizaino įrankyje.

Jei norite, kad vartotojai matytų ataskaitų sritį, kurią nustatėte kaip numatytąjį organizacijos, galite:

* Nustatyti, kad ataskaitų sritis būtų "Sitemap"

* Prieigos prie "Sitemap" apibrėžtosios ataskaitų srities pašalinimas tiems vartotojams
