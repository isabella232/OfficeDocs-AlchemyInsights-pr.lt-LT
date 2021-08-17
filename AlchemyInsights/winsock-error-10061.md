---
title: 1554 Winsock klaida 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083238"
---
# <a name="winsock-error-10061"></a>Winsock error 10061

Šis klaidos kodas reiškia, kad "Microsoft" nepavyko nustatyti TCP lizdo (ryšio) su tiksliniu pagrindinio kompiuterio. Labiausiai tikėtina šios klaidos priežastis yra užkardos konfigūravimo problema. Norėdami išspręsti problemą, patikrinkite šiuos parametrus:

- Patikrinkite užkardos konfigūraciją naudodami [informaciją, Microsoft 365 URL ir IP adresų diapazonuose](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jei klaida yra konkreti Exchange Online Protection (EOP), jums anksčiau turėjo būti pranešta apie ip [adresų Exchange Online Protection pakeitimą.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Patikrinkite, ar jūsų interneto paslaugų teikėjas (ISP) neblokuoja prievado.

- Patikrinkite išmaniojo pagrindinio kompiuterio ir paskirties serverio parametrus jungtyse.

Atkreipkite dėmesį Microsoft 365 kad taip *neblokuoja* gaunamų ryšių.
