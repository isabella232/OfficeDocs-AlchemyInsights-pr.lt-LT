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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="ff28d-102">EWS ribojimo parametrų keitimas</span><span class="sxs-lookup"><span data-stu-id="ff28d-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="ff28d-103">Paleiskite mūsų automatizuotą testą, kuris leis jums modifikuoti EWS ribojimo strategiją perkėlimo metu.</span><span class="sxs-lookup"><span data-stu-id="ff28d-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="ff28d-104">Atkreipkite dėmesį, kad net ir įvykdžius šį testą, EWS importavimui vis tiek bus taikomas iki 150 MB per 5 minutes apribojimas kiekvienai pašto dėžutei; norėdami pasiekti didesnį perkėlimo pralaidumo greitį, vienu metu perkelkite daugiau vartotojų.</span><span class="sxs-lookup"><span data-stu-id="ff28d-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="ff28d-105">Atkreipkite dėmesį, kad EWS ribojimo strategijos pakeitimai netaikomi šiems perkėlimo tipams (naudojant „Microsoft“ įrankius): hibridinis, visiškasis / dalinis (RPC / HTTP), IMAP, „G Suite“, viešasis aplankas arba PST importavimo tarnyba.</span><span class="sxs-lookup"><span data-stu-id="ff28d-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>