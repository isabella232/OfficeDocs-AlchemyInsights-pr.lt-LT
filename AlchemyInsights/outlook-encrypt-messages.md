---
title: S/MIME internetinė "Outlook"
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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010732"
---
# <a name="encrypt-email-messages-in-outlook"></a>El. laiškų šifravimas Outlook

Microsoft 365 Pranešimų šifravimas sukurtas naudojant "Microsoft Azure Rights Management" ("Azure RMS"), kuri yra "Azure" informacijos apsaugos dalis. Jei jūsų prenumeratoje yra "Azure Rights Management" arba "Azure" informacijos apsauga, jums nereikia atlikti jokių veiksmų, kad teisių valdymo tarnyba **būtų įjungiama** arba suaktyvinamas rankiniu būdu.

Atsižvelgdami į klientų atsiliepimus, nebegalėsime Exchange pašto srauto taisykles automatiškai šifruoti siunčiamus el. laiškus, kuriuose pagal numatytuosius nustatymus jūsų nuomotojas turi tam tikro tipo slaptą informaciją. Vietoj to pateikiame išsamias instrukcijas, kaip tai padaryti patys. Daugiau informacijos apie tai, kaip sukurti transportavimo taisyklę slaptai informacijai šifruoti, žr. [šiame straipsnyje](https://aka.ms/OmeEtr).

- Jei naudojate Outlook (anksčiau **– OWA):** Kurdami el. laišką tiesiog spustelėkite **Apsaugoti** OWA. Tai bus taikoma "Neadresuoti" teisių. Spustelėkite **Keisti teises ir** pasirinkite Šifruoti, kad šifruotų tik pranešimą. 

- Jei naudojate **"Outlook"** klientą: norėdami siųsti šifruotą pranešimą iš "Outlook 2013" arba "Outlook 2016 for Mac", pasirinkite Parinktys teisės , tada pasirinkite  >  norimą apsaugos parinktį.

- Norėdami **automatiškai šifruoti** visus el. laiškus, siunčiamus tam tikriems gavėjams arba išorinėms partnerių organizacijoms, turite sukurti pašto srauto transportavimo taisyklę Exchange administravimo centre. Išsamios instrukcijos pateikiamos šiame [palaikymo straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

