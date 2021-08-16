---
title: "\"Dynamics 365\" – netinkama ataskaitų sritis rodoma \"Dynamics 365\" vieningojoje sąsajoje"
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101490"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Netinkama ataskaitų sritis rodoma "Dynamics 365" vieningojoje sąsajoje

Yra kelios priežastys, kodėl galite matyti kitą ataskaitų sritį nei tikitės:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Vartotojas nustatė vartotojo numatytąją ataskaitų sritį 

Paprastai galite nustatyti vartotojo numatytąją ataskaitų sritį, jei **ataskaitų** srities komandų juostoje nerodo mygtuko Nustatyti kaip numatytąjį. Vartotojo numatytoji ataskaitų sritis perrašys visas kitas numatytąsias ataskaitų sritis, net jei vartotojo numatytoji ataskaitų sritis nėra dabartinėje programoje.

Norėdami nustatyti numatytąją ataskaitų sritį, naudokite toliau nurodytą sprendimo būdą.

1. Sukurkite naują asmeninę ataskaitų sritį.

2. Nustatykite tą naują ataskaitų sritį kaip vartotojo numatytąjį.

3. Panaikinkite tą ataskaitų sritį.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Ataskaitų sritis nustatyta svetainės struktūroje

Gali būti, kad nustatėte organizacijos numatytąją ataskaitų sritį pasirinkdami ataskaitų sritį ir pasirinkdami "Nustatyti kaip numatytąjį" dalyje "Tinkinti sistemą". Tačiau svetainės struktūros dizaino įrankyje apibrėžta ataskaitų sritis bus viršesnė už šią ataskaitų sritį, jei vartotojas turi prieigą prie jos.

Norėdami, kad vartotojai galėtų matyti ataskaitų sritį, kurią nustatėte kaip numatytąją organizaciją, galite:

* Ataskaitų srities nustatymas svetainės struktūroje

* Prieigos prie svetainės schemos apibrėžtos ataskaitų srities pašalinimas tiems vartotojams
