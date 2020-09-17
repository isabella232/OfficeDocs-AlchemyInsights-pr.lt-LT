---
title: 1065 nuteistųjų iš "IOP" siuntimo IP adreso rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806803"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>"IOP" siunčiamų IP adreso diapazonų nuteistųjų uždraudimas

Aptikome galimą organizacijos problemą, kuri (jei nepataisoma spalio 26 d., 2018) gali pažeisti pašto srautą į vietinę arba išorinę paskirties vietą. Kaip buvo pranešta anksčiau, Norėdami supaprastinti IP adresų diapazono valdymą, mes konsoliduojame "Exchange Online Protection" ("e") IP adresų diapazonus, kurie naudojami siųsti ir gauti el. laiškus už "Microsoft 365". Mūsų analizė rodo, kad vienas ar daugiau išorinių elektroninio pašto šaltinių arba paskirties vietų, kurias sukonfigūravote pašto srauto jungtuse, nepriima ryšių iš [čia](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)rodomų IP adresų diapazonų.

Veikti iki spalio 26 d., siekiant užtikrinti, kad šie šaltiniai ir miestai sutiktų ryšius su visais [paskelbtais EOP IP adresais](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ir iš jų.

Daugiau informacijos apie šį keitimą ieškokite pranešimų centro pranešimų [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Pastaba**: jei anksčiau naudojote IP arba URL skelbimą naudodami HTML, XML ir RSS galinio punkto naujinimus, taip pat turite perkelti į naujas žiniatinklio tarnybas, kad automatizuodami šio tipo naujinimus. Daugiau informacijos ieškokite ["microsoft 365" galinio punkto kategorijų ir "microsoft 365" IP adreso ir URL žiniatinklio tarnybos](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
