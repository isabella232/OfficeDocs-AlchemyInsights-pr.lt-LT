---
title: EWS ribojimo parametrų keitimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818044"
---
# <a name="changing-ews-throttling-settings"></a>EWS ribojimo parametrų keitimas

Paleiskite mūsų automatizuotą testą, kuris leis jums modifikuoti EWS ribojimo strategiją perkėlimo metu. Atkreipkite dėmesį, kad net ir įvykdžius šį testą, EWS importavimui vis tiek bus taikomas iki 150 MB per 5 minutes apribojimas kiekvienai pašto dėžutei; norėdami pasiekti didesnį perkėlimo pralaidumo greitį, vienu metu perkelkite daugiau vartotojų.

Atkreipkite dėmesį, kad EWS ribojimo strategijos pakeitimai netaikomi šiems perkėlimo tipams (naudojant „Microsoft“ įrankius): hibridinis, visiškasis / dalinis (RPC / HTTP), IMAP, „G Suite“, viešasis aplankas arba PST importavimo tarnyba.