---
title: Numatytasis Outlook parametras netaikomas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454750"
---
# <a name="default-outlook-label-setting-not-applied"></a>Numatytasis Outlook parametras netaikomas

Jei jūsų Outlook numatytieji etikečių parametrai netinkamai taikomi ir taikoma kita etiketė arba netaikoma jokia etiketė, gali būti, kad iškilo žinoma problema (MC277818) ir turėtumėte atlikti vieną iš šių 2 parinkčių, kad išspręsite problemą:

**1 parinktis:**

1. Eikite į Microsoft 365 centro > **sprendimų informacijos**  >  **apsaugą.**
1. Pasirinkite **Etikečių** strategijos ir pasirinkite norimą redaguoti etikečių strategiją (**"OutlookDefaultlabel"** parametras nėra tinkamai nustatytas tam tikrai etikečių strategijai. Paleiskite **Get-labelpolicy,** kad galėtumėte peržiūrėti šį parametrą), tada **pasirinkite Redaguoti strategiją**.
1. Pasirinkite **Pirmyn,** kol pamatysite parametrą Taikyti šią numatytąją etiketę  el. laiškams **,** kuris pasiekiamas, jei dialogo lange Strategijos parametrai pasirinksite Reikalauti, kad vartotojai pritaikytumėte etiketę įstatų el. laiškams **ir** dokumentams.
1. Dialogo **lange Taikyti numatytąją etiketę** dokumentams išplečiamajame **sąraše** pasirinkite Nėra.
1. Pasirinkite **Pirmyn** ir **Pateikti, kad** įrašytumėte etiketės parametrus.

**2 parinktis:**

["PowerShell"](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)saugos ir atitikties centre naudokite "Set-LabelPolicy commandlet" norėdami pakeisti **"OutlookDefaultlabel"** **į Nėra** {OutlookDefaultLabel="None"}.

Vykdyti: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Daugiau informacijos apie numatytąsias Outlook, žr. Kitos [numatytosios](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)etiketės nustatymas Outlook .