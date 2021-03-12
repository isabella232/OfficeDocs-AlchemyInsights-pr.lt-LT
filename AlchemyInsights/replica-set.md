---
title: Replikų rinkinys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714251"
---
# <a name="replica-set"></a>Replikų rinkinys

"AADDS" taip pat vadinama valdomu domenu. Tai iš tikrųjų yra du domeno valdikliai, kurie vykdomi ir prižiūrimi backend. Du DC apima vieną pagrindinį DC ir vieną replikavimo DC. Atsarginės kopijos, esančios AADDS (valdomas domenas), yra automatinis procesas, kurį tvarko "Azure" platforma. Kilus problemai su valdomu domenu, "Azure" palaikymas gali padėti atkurti atsarginę kopiją.

Sukuriate kiekvieną replikų rinkinį virtualiame tinkle. Kiekvienas virtualusis tinklas turi būti valdomas visiems kitiems virtualiam tinklui, kuriame yra valdomo domeno replikų rinkinys. Ši konfigūracija sukuria tinklinio tinklo topologiją, kuri palaiko katalogų replikavimą. Virtualiame tinkle gali būti palaikomi keli replikų rinkiniai, jei kiekvienas replikų rinkinys yra kitame virtualiame potinklyje.

Daugiau informacijos apie replikų rinkinį ieškokite [koncepcijų replikų rinkiniai](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
