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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110688"
---
# <a name="replica-set"></a>Replikų rinkinys

AADDS taip pat vadinama valdomą domenu. Iš tikrųjų tai yra du domeno valdikliai, kuriuos valdo ir tvarko vidinė sąsaja. Du DC apima vieną pagrindinę DC ir vieną replikavimo DC. AADDS (valdomo domeno) atsarginės kopijos yra automatizuotas procesas, kurį valdo "Azure" platforma. Jei kyla jūsų valdomo domeno problema, "Azure" palaikymas gali padėti atkurti iš atsarginės kopijos.

Kiekvieną replikų rinkinį sukuriate virtualiame tinkle. Kiekvienas virtualusis tinklas turi būti lygiaverčiai mazgams prie kiekvieno kito virtualaus tinklo, kuriame yra valdomo domeno replikų rinkinys. Ši konfigūracija sukuria tinklo tinklo topologiją, palaikančią katalogų replikavimą. Virtualusis tinklas gali palaikyti kelis replikų rinkinius, jei kiekvienas replikų rinkinys yra skirtingame virtualiame potinklyje.

Daugiau informacijos apie replikų rinkinį žr. [Sąvokų replikų rinkiniai](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
