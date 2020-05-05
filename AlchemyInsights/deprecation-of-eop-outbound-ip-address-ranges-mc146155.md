---
title: 1065 EOP siunčiamo IP adreso diapazonųMC146155 nuvertėjimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704605"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP siunčiamų IP adresų diapazonų nuvertėjimas

Aptikome galimą jūsų organizacijos problemą, kuri (jei nebus ištaisyta iki 2018 m. spalio 26 d.) gali nutraukti pašto srautą į vietines arba išorines paskirties vietas. Kaip anksčiau pranešta, siekiant supaprastinti IP adresų diapazono valdymą, konsoliduojame "Exchange Online Protection" (EOP) IP adresų diapazonus, naudojamus el. laiškams siųsti ir gauti už "Microsoft 365" ribų. Mūsų analizė rodo, kad vienas ar daugiau išorinių el. pašto šaltinių ar paskirties vietų, kurias sukonfigūravote pašto srauto jungtyse, nepriima ryšių iš [ČIA](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)rodomų IP adresų diapazonų .

Veikti iki spalio 26 d., siekiant užtikrinti, kad šie šaltiniai ir paskirties vietos priims ryšius su visais [paskelbtais EOP IP adresais](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ir iš jų .

Jei norite gauti daugiau informacijos apie šį pakeitimą, peržiūrėkite pranešimų centro pranešimų [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Pastaba**: jei anksčiau naudojote IP arba URL publikavimą per HTML, XML ir RSS galinio punkto naujinimams, taip pat turėtumėte pereiti prie naujų žiniatinklio tarnybų, kad automatizuotumėte šių tipų naujinimus. Daugiau informacijos ieškokite ["Microsoft 365" galinių punktų kategorijos ir "Microsoft 365" IP adresas ir URL žiniatinklio tarnyba](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
