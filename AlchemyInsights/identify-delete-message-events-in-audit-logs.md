---
title: Pranešimų naikinimo įvykių atpažinimas audito žurnaluose
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696521"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Panaikintų el. laiškų audito žurnalai

Nuo sausio 2019 d. "Microsoft" pagal numatytuosius numatytuosius pašto dėžučių audito žurnalus įjunkite. Kitu atveju Norėdami peržiūrėti konkretaus vartotojo panaikintų pranešimų įvykius, turite rankiniu būdu įgalinti tikrinimo veiksmų naikinimo veiksmus. Jei pašto dėžutės audito registravimas jau įgalintas jūsų organizacijai arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.

1. Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/)

2. Spustelėkite **ieška ir tyrimas** ir pasirinkite **audito žurnalų ieška**.

3. Laukuose **pradžios data** ir **pabaigos data** pasirinkite datų intervalą. Nurodo vartotojo, kurį norite analizuoti, vartotojo vardą (vartotojas, kuris panaikino elementus). Lauke **veikla** pasirinkite **pašalinti laiškai iš panaikintų elementų aplanko** ir **perkelti laiškus į aplanką Panaikinta**.

4. Spustelėkite **ieška**.

Rezultatuose pasirinkite audito įrašą. Išsamios informacijos išskridimas spustelėkite **daugiau informacijos**. Papildoma informacija apie panaikintą elementą (pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas) rodoma lauke **Affecteditems** . Ypatybė **Clientinfostring** bus rodoma, jei jis buvo panaikintas programoje "Outlook", "Outlook" žiniatinklyje (anksčiau – "Outlook Web App") arba bet kurį kitą įrenginį.

Daugiau informacijos ieškokite kaip [nustatyti, kas nustato pašto dėžutės pašto peradresavimą](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Pastaba**: panaikintų elementų atkurti negalima naudojant audito žurnalų funkciją. Norėdami atkurti panaikintus laiškus internetinėje "Outlook", peržiūrėkite [panaikintų elementų atkūrimas "Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)".
