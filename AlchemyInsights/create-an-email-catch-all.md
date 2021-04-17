---
title: El. laiško užgaudo kūrimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816208"
---
# <a name="create-an-email-catch-all"></a>El. laiško užgaudo kūrimas

Laimikio naudojimas yra labai neskatinantis. Geriau pateikti siuntėjui atšokti, kad siuntėjai žinotų, jog jų laiško nepavyko pristatyti kaip adreso, kad jie galėtų imtis veiksmų. Taip pat galite apriboti stebimos pašto dėžutės gaudo tik anksčiau galiojančius el. pašto adresus. 

Visos pašto dėžutės gaus daug pašto šiukšlių ir galiausiai gali užpildyti, jei nebus atidžiai stebimos. (Yra gavimo apribojimų.) 

Jei nuspręsite tęsti, atlikite šiuos veiksmus:

1. Dinaminio paskirstymo grupės kūrimas & "Visi gavėjų tipai".

2. Sukurkite specialią pašto dėžutę, kad gaudysite el. laiškus, pvz., catchall@domain.com.

3. Konkretaus domeno domeno tipą nustatykite kaip "InternalRelay". Jei vėliau pašalinsite viską, įsitikinkite, kad domenas vėl bus patikimas.

4. Sukurkite "Mailflow" transportavimo taisyklę taip:

    - Jei siuntėjas yra "Už organizacijos ribų"
    - Peradresuoti laišką į Catchall@domain.com
    - Išskyrus atvejus, kai gavėjas yra allusers@domain.com narys (siuntimo grupėje yra visi nariai)
    - Įsitikinkite, kad į dinaminio paskirstymo grupę įtraukta naujų pašto dėžučių
