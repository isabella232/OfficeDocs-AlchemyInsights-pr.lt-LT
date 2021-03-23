---
title: Importavimas ir eksportavimas iš "Yammer"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036121"
---
# <a name="import-and-export-from-yammer"></a>Importavimas ir eksportavimas iš "Yammer"

**Importuoti**

Vartotojo importavimo parinktys gali skirtis, atsižvelgiant į tai, ar jūsų "Yammer" tinklas yra [vietinis režimas, skirtas "Microsoft 365"](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), ar ne.

- **Neprigimtinis režimas**: vartotojus galima importuoti į grupes naudojant " [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) " ("100" vartotojų) grupės parametruose arba tinkle naudojant [masinį naujinimą](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) tinklo administratorius.
- **Prigimtinis režimas**: grupės narystė ir tinklo narystės operacijos turi būti atliekamos iš ["Microsoft" 365 administravimo portalo, "](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD" portalo](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)arba naudojant kitą "Azure AD" parinktį. Vietiniu režimu esantys tinklai nebeturi prieigos prie masinio naujinimo ir kitų senstelėjusių funkcijų.

> [!IMPORTANT]
> "Yammer" niekada nepalaikė turinio importavimo iš tinklo administratoriaus net tada, kai duomenų eksportavimo funkcija buvo naudota kitame tinkle. Turinys gali būti iš naujo paskelbtas partnerių sprendimais arba "Yammer" kitų API.

**Eksportuoti**

[Eksportuokite tinklo duomenis tinklo administratorius](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) leidžia eksportuoti turinį iš "Yammer" tinklų, įskaitant pranešimą ir failus. Priedai gali būti labai dideli ir dėl to eksportuos gali užtrukti, kol bus baigta. Rekomenduojame, kad aktyvūs tinklai būtų eksportuojami naudojant [duomenų eksportavimo API](https://developer.yammer.com/docs/data-export-api) į gabaliukus pagal dieną ar savaitę. "Microsoft" palaikymas neteikia šio tikslo pasirinktiniams scenarijams.

Atskiras [Gdpr eksportavimas](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) yra skirtas atskiro vartotojo turiniui eksportuoti.