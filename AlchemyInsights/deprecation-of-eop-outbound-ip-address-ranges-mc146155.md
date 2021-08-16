---
title: 1065 EOP siunčiamų IP adresų diapazonų atėmimasMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031270"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP siunčiamų IP adresų diapazonų atėmimas

Aptikome galimą problemą su jūsų organizacija, kuri (jei neištaisyta iki 2018 m. spalio 26 d.) gali nutraukti pašto srautą į jūsų vietinį arba išorinį paskirties vietą. Kaip anksčiau buvo pranešta, kad būtų supaprastintas IP adresų diapazono valdymas, mes konsoliduojame "Exchange Online Protection" (EOP) IP adresų diapazonus, kurie naudojami siųsti ir gauti el. laiškus ne Microsoft 365. Mūsų analizė rodo, kad vienas ar daugiau išorinių el. pašto šaltinių arba paskirties vietų, kurias sukonfigūravote pašto srauto jungtyse, nepriima ryšių iš ČIA rodomo IP adresų [diapazonų.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Veikite iki spalio 26 d., kad užtikrinsite, jog šie šaltiniai ir paskirties vietos priims ryšius su visais [paskelbtais EOP IP adresais ir iš jų.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Daugiau informacijos apie šį keitimą žr. Pranešimų centro įrašai [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Pastaba:** jei anksčiau naudojote IP arba URL publikavimą html, XML ir RSS pabaigos taško naujinams, taip pat turėtumėte pereiti į naujas žiniatinklio tarnybas, kad automatizuotų šių tipų naujinimus. Daugiau informacijos žr. [Microsoft 365 pabaigos taško kategorijas ir Microsoft 365 IP adresą ir URL žiniatinklio tarnybą](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
