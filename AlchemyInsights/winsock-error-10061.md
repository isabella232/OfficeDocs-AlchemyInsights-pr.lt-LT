---
title: 1554 Winsock klaida 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757108"
---
# <a name="winsock-error-10061"></a>Winsock klaida 10061

Ši klaida reiškia, kad "Office 365" negalėjo sukurti TCP socket (jungtis) su tikslinės priimančiosios. Labiausiai tikėtina, dažniausia šios klaidos priežastis yra ugniasienės konfigūracijos problema. Norėdami išspręsti šią problemą, patikrinkite šiuos parametrus:

- Patikrinkite, ar jūsų ugniasienės konfigūracijos informacija iš [Office 365 URL ir IP adresų diapazonas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jei klaidos yra susijusios su Exchange Online Protection (EOP), jums turėtų anksčiau pranešama apie pasikeičia į [Exchange Online apsaugos IP adresus](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Įsitikinkite, kad jūsų interneto paslaugų teikėjas (ISP) neblokuoja uosto.

- Patikrinkite, ar protingas pagrindinio kompiuterio ir paskirties serverio parametrus jūsų jungtys.

Atkreipkite dėmesį, kad "Office 365" ne blokuoti *priimamus* ryšius, tokiu būdu.
