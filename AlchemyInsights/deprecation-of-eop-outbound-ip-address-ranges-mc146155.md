---
title: 1065 EOP nuteistųjų siuntimo IP adresas rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752963"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Nuteistųjų, EOP siuntimo IP adresų diapazonai

Aptikome galima problema su jūsų organizacija, kuri (jei negali ištaisyti iki 2018 m. spalio 26 d.) gali sugadinti pašto srautas į jūsų vietinėje ar išorės šalis ir miestus. Kaip anksčiau bendravo, supaprastinti IP adresų diapazoną valdymo, mes konsoliduojate Exchange Online Protection "(EOP) IP adresų diapazonus, kurie yra naudojami siųsti ir gauti el. laiškus ne iš" Office 365 ". Mūsų analizė rodo, kad vienas ar daugiau iš išorės paštu šaltinių ar paskirties vietą, sukonfigūravę pašto srauto jungtys nėra priimti ryšių iš to IP adreso diapazonų parodyta [čia](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Veikia iki spalio 26 užtikrinti šių šaltinių ir miestai bus priimti ryšius į ir iš visų [paskelbtas EOP IP adresus](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Daugiau informacijos apie šį keitimą, žiūrėkite pranešimų centras registruoja [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Pastaba**: jei anksčiau naudojote IP arba URL leidyba per HTML, XML, ir RSS galinio punkto naujinimų, jūs taip pat turi pereiti prie naujų interneto paslaugų automatizavimo šių tipų naujinimus. Norėdami gauti daugiau informacijos, peržiūrėkite ["Office 365" galinio punkto kategorijos ir Office 365 IP adresą ir URL interneto paslaugos](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
