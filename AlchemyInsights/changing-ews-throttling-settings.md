---
title: EWS ribojimo parametrų keitimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075905"
---
# <a name="changing-ews-throttling-settings"></a>EWS ribojimo parametrų keitimas

Paleiskite mūsų automatizuotą testą, kuris leis jums modifikuoti EWS ribojimo strategiją perkėlimo metu. Atkreipkite dėmesį, kad net ir įvykdžius šį testą, EWS importavimui vis tiek bus taikomas iki 150 MB per 5 minutes apribojimas kiekvienai pašto dėžutei; norėdami pasiekti didesnį perkėlimo pralaidumo greitį, vienu metu perkelkite daugiau vartotojų.

Atkreipkite dėmesį, kad EWS ribojimo strategijos pakeitimai netaikomi šiems perkėlimo tipams (naudojant "Microsoft" įrankius): hibridinis, visiškasis / dalinis (RPC / HTTP), IMAP, „G Suite“, viešasis aplankas arba PST importavimo tarnyba.