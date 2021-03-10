---
title: MDATP išimčių konfigūravimas ir patvirtinimas "Linux" įrenginyje
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696076"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="34af4-102">MDATP išimčių konfigūravimas ir patvirtinimas "Linux" įrenginyje</span><span class="sxs-lookup"><span data-stu-id="34af4-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="34af4-103">Galite išskirti tam tikrus failus, aplankus, procesus ir procesą atidarytus failus iš MDATP nuskaito.</span><span class="sxs-lookup"><span data-stu-id="34af4-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="34af4-104">Išimtys padeda išvengti neteisingo jūsų organizacijos programinės įrangos ir failų aptikimo.</span><span class="sxs-lookup"><span data-stu-id="34af4-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="34af4-105">Išimtys taip pat padeda sušvelninti MDATP veikimo problemas.</span><span class="sxs-lookup"><span data-stu-id="34af4-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="34af4-106">Norėdami sužinoti daugiau, peržiūrėkite [išimčių, skirtų "Linux" MDATP, konfigūravimą ir įteisinimo](https://go.microsoft.com/fwlink/?linkid=2144517)galimybę.</span><span class="sxs-lookup"><span data-stu-id="34af4-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="34af4-107">Šiame straipsnyje aprašytos išimtys netaikomos kitoms "Linux" MDATP, įskaitant galinio punkto aptikimo ir reagavimo (EDR), galimybėms.</span><span class="sxs-lookup"><span data-stu-id="34af4-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="34af4-108">Failai, kuriuos neįtrauksite naudodami šiame straipsnyje aprašytus metodus, vis tiek gali sukelti EDR įspėjimus ir kitas aptikimo galimybes.</span><span class="sxs-lookup"><span data-stu-id="34af4-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
