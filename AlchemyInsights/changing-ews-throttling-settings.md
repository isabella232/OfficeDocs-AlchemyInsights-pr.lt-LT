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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968385"
---
# <a name="changing-ews-throttling-settings"></a>EWS ribojimo parametrų keitimas

Paleiskite mūsų automatizuotą testą, kuris leis jums modifikuoti EWS ribojimo strategiją perkėlimo metu. Atkreipkite dėmesį, kad net ir įvykdžius šį testą, EWS importavimui vis tiek bus taikomas iki 150 MB per 5 minutes apribojimas kiekvienai pašto dėžutei; norėdami pasiekti didesnį perkėlimo pralaidumo greitį, vienu metu perkelkite daugiau vartotojų.

Atkreipkite dėmesį, kad EWS ribojimo strategijos pakeitimai netaikomi šiems perkėlimo tipams (naudojant „Microsoft“ įrankius): hibridinis, visiškasis / dalinis (RPC / HTTP), IMAP, „G Suite“, viešasis aplankas arba PST importavimo tarnyba.