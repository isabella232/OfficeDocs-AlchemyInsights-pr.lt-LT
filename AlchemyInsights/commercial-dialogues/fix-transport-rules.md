---
title: Taisykite transportavimo taisykles
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750581"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="8147f-102">Taisykite transportavimo taisykles</span><span class="sxs-lookup"><span data-stu-id="8147f-102">Fix transport rules</span></span>

<span data-ttu-id="8147f-103">Pasirinktinio pašto srauto taisyklė turi įtakos šiam pranešimui.</span><span class="sxs-lookup"><span data-stu-id="8147f-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="8147f-104">Norėdami peržiūrėti tikslią taisyklę, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8147f-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="8147f-105">Pateikimo rezultatuose, dalyje **papildoma informacija**, pasižymėkite **GUID** arba **strategijos pavadinimą**.</span><span class="sxs-lookup"><span data-stu-id="8147f-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="8147f-106">"Exchange Management Shell" Paleistis.</span><span class="sxs-lookup"><span data-stu-id="8147f-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="8147f-107">Daugiau informacijos ieškokite " [Exchange" valdymo aplinkos atidarymas](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="8147f-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="8147f-108">Vykdykite šią komandą (naudodami savo pateiktyje esantį GUID):  **get-TransportRule-tapatybė "GUID" | FL \* aprašas**\*</span><span class="sxs-lookup"><span data-stu-id="8147f-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="8147f-109">Peržiūrėkite aprašą ir peržiūrėkite sukonfigūruotas sąlygas, kurios paveikė laišką.</span><span class="sxs-lookup"><span data-stu-id="8147f-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="8147f-110">Norėdami sužinoti daugiau, peržiūrėkite [get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="8147f-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
