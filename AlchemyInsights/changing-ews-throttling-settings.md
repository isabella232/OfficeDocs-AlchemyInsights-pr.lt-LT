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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="c9eda-102">EWS ribojimo parametrų keitimas</span><span class="sxs-lookup"><span data-stu-id="c9eda-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="c9eda-103">Paleiskite mūsų automatizuotą testą, kuris leis jums modifikuoti EWS ribojimo strategiją perkėlimo metu.</span><span class="sxs-lookup"><span data-stu-id="c9eda-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="c9eda-104">Atkreipkite dėmesį, kad net ir įvykdžius šį testą, EWS importavimui vis tiek bus taikomas iki 150 MB per 5 minutes apribojimas kiekvienai pašto dėžutei; norėdami pasiekti didesnį perkėlimo pralaidumo greitį, vienu metu perkelkite daugiau vartotojų.</span><span class="sxs-lookup"><span data-stu-id="c9eda-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="c9eda-105">Atkreipkite dėmesį, kad EWS ribojimo strategijos pakeitimai netaikomi šiems perkėlimo tipams (naudojant „Microsoft“ įrankius): hibridinis, visiškasis / dalinis (RPC / HTTP), IMAP, „G Suite“, viešasis aplankas arba PST importavimo tarnyba.</span><span class="sxs-lookup"><span data-stu-id="c9eda-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>