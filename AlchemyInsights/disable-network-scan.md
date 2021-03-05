---
title: Išjungti tinklo nuskaitymą
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481966"
---
# <a name="disable-network-scan"></a><span data-ttu-id="0f84e-102">Išjungti tinklo nuskaitymą</span><span class="sxs-lookup"><span data-stu-id="0f84e-102">Disable network scan</span></span>

<span data-ttu-id="0f84e-103">Tinklo bendrinimo skenavimas gali turėti įtakos našumui.</span><span class="sxs-lookup"><span data-stu-id="0f84e-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="0f84e-104">Norėdami užtikrinti, kad klientas nenuskaito tinklo bendrinimo/failų pagal numatytuosius parametrus, sukonfigūruokite šiuos "Windows" sargybos taikomosios programos parametrus kaip **True**:</span><span class="sxs-lookup"><span data-stu-id="0f84e-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="0f84e-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="0f84e-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="0f84e-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="0f84e-106">DisableScanningNetworkFiles</span></span>