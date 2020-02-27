---
title: Sukurkite el. Laiško sugavimo viską
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286200"
---
# <a name="create-an-email-catch-all"></a>Sukurkite el. Laiško sugavimo viską

Laimikio naudojimas yra labai varžomas. Geriau pateikti atmetimą siuntėjui, kad siuntėjai žinotų, jog jų pranešimas negali būti pristatytas taip, kaip sprendžiama, kad jie galėtų imtis veiksmų. Taip pat galite apriboti stebimą pašto dėžutę tik sugavimo tik anksčiau galiojančius el. pašto adresus. 

Bet koks laimikis visos pašto dėžutės gaus nemažai šlamštas ir galiausiai gali užpildyti, jei nėra atidžiai stebimi. (Yra gavimo ribos.) 

Jei nuspręsite tęsti, atlikite šiuos veiksmus:

1. Dinaminio paskirstymo grupės kūrimas & apima "Visi gavėjų tipai".

2. Sukurkite specialią pašto dėžutę el. laiškams sugauti, pvz., catchall@domain.com.

3. Konkretaus domeno, nustatykite DomainType į "InternalRelay". Jei vėliau pašalinsite visus sugavimus, būtinai nustatykite domeną atgal į Autoritetingą.

4. Sukurkite Mailflow transportavimo taisyklę taip:

    - Jei siuntėjas yra "už organizacijos ribų"
    - Peradresuoti pranešimą į Catchall@domain.com
    - Išskyrus atvejus, kai gavėjas yra allusers@domain.com narys (paskirstymo grupėje yra visi nariai)
    - Įsitikinkite, kad patikrinti, ar naujos pašto dėžutės yra įtrauktos į dinaminio paskirstymo grupės
