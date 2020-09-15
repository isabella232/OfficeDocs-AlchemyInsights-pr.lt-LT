---
title: El. laiško kūrimas visiems
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712994"
---
# <a name="create-an-email-catch-all"></a>El. laiško kūrimas visiems

Naudokite sugavimo visi primygtinai nenori. Jei norite, kad būtų lengviau grįžti prie siuntėjo, pranešantiems siuntėjams žinotų, kad pranešimo negalima pristatyti, kad jie galėtų imtis veiksmų. Taip pat galite apriboti stebimą pašto dėžutę, kad tik galėtumėte sugauti anksčiau galiojančius el. pašto adresus. 

Bet koks laimikis visos pašto dėžutės gaus gerą pašto šiukšlių ir galiausiai gali būti užpildytas, jei nėra atidžiai stebimas. (Yra gaunamų apribojimų.) 

Jei nuspręsite tęsti, atlikite šiuos veiksmus:

1. Dinaminio paskirstymo grupės kūrimas & įtraukti "visi gavėjų tipai".

2. Sukurkite specialią pašto dėžutę, kad galėtumėte sugauti laiškus, pvz., catchall@domain.com.

3. Konkrečiam domenui nustatykite DomainType "InternalRelay". Jei po to norite pašalinti viską, įsitikinkite, kad domeną norite grąžinti į patikimą.

4. Sukurkite pašto srauto transportavimo taisyklę taip:

    - Jei siuntėjas yra "už organizacijos ribų"
    - Peradresuokite pranešimą į "Catchall@domain.com"
    - Išskyrus atvejus, kai gavėjas yra "allusers@domain.com" narys (paskirstymo grupėje yra visi nariai)
    - Įsitikinkite, kad patvirtintumėte, jog naujos pašto dėžutės įtraukiamos į dinaminio paskirstymo grupę
