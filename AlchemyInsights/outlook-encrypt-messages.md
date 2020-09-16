---
title: S/MIME "Outlook" žiniatinklyje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772306"
---
# <a name="encrypt-email-messages-in-outlook"></a>El. laiškų šifravimas programoje "Outlook"

"Microsoft 365" pranešimų šifravimas yra sukurtas "Microsoft Azure Rights Management" ("Azure RMS"), kuris yra "Azure" informacijos apsaugos dalis. Jei jūsų produktų pakete yra "Azure Rights Management" arba "Azure" informacijos apsauga, **jums nereikia imtis jokių veiksmų, kad rankiniu būdu įgalintumėte arba suaktyvintumėte** teisių valdymo tarnybą.

Atsižvelgdami į klientų atsiliepimus, nebegalėsite įgalinti "Exchange" pašto srauto taisyklių, kad automatiškai šifruotų siunčiamus laiškus, kuriuose yra tam tikro tipo slaptos informacijos pagal numatytuosius reikalavimus. Vietoj to, mes teikiame išsamias instrukcijas, kaip galite tai padaryti patys. Daugiau informacijos apie tai, kaip sukurti transportavimo taisyklę, kad užšifruotų slaptą informaciją, rasite [šiame straipsnyje](https://aka.ms/OmeEtr).

- Jei naudojate "Outlook" žiniatinklyje (anksčiau **OWA**): kurdami el. laišką, tiesiog spustelėkite **apsaugoti** OWA. Tai bus taikoma "Nepersiųskite" leidimo. Spustelėkite **Keisti teises** ir pasirinkite **šifruoti** , kad būtų šifruojamas tik pranešimas.

- Jei naudojate **"Outlook Client**": Norėdami nusiųsti šifruotą pranešimą iš "Outlook" 2013 arba "2016" arba "Outlook 2016 for Mac", pasirinkite **parinkčių**  >  **teisės**, tada pasirinkite reikiamą apsaugos parinktį.

- Norėdami **automatiškai šifruoti visus el. laiškus** , siunčiamus tam tikriems gavėjams arba išoriniams partnerių organizacijoms, turite sukurti pašto srauto taisyklę "Exchange" administravimo centre. [Šiame palaikymo straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)pateikiamos išsamios instrukcijos.

