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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698870"
---
# <a name="winsock-error-10061"></a>Winsock klaida 10061

Šis klaidos kodas reiškia, kad "Microsoft" negalėjo sukurti TCP lizdo (ryšio) su paskirties pagrindiniu kompiuteriu. Labiausiai tikėtina šios klaidos priežastis yra jūsų užkardos konfigūravimo problema. Norėdami išspręsti problemą, patikrinkite šiuos parametrus:

- Patikrinkite užkardos konfigūraciją naudodami ["Microsoft 365" URL ir IP adresų diapazonų](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) informaciją

- Jei klaida būdinga "Exchange Online Protection" ("e"), prieš tai turite pranešti apie " [Exchange Online Protection" IP adresų](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)pakeitimą.

- Patikrinkite, ar jūsų interneto paslaugų teikėjas (ISP) neužblokuoja prievado.

- Įsitikinkite, kad "Smart Host" ir paskirties serverio parametrai yra jūsų jungtyje.

Nepamirškite, kad "Microsoft 365" neblokuoja *įeinančių* ryšių šiuo būdu.
