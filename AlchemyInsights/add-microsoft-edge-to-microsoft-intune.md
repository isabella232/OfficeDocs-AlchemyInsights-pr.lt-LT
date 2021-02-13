---
title: "\"Microsoft Edge\" įtraukimas į \"Microsoft Intune\""
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194513"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="d96dc-102">"Microsoft Edge" įtraukimas į "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="d96dc-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="d96dc-103">Norėdami įdiegti, konfigūruoti, stebėti ir apsaugoti "Microsoft Edge", skirtą "Windows 10", pirmiausia turite įtraukti jį į "Microsoft Intune".</span><span class="sxs-lookup"><span data-stu-id="d96dc-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="d96dc-104">Intune palaiko "Microsoft Edge" 77 ir vėlesnes versijas.</span><span class="sxs-lookup"><span data-stu-id="d96dc-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="d96dc-105">Intune aptiks bet kokius iš anksto esamus "Microsoft Edge" diegimus.</span><span class="sxs-lookup"><span data-stu-id="d96dc-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="d96dc-106">Jei "Microsoft Edge" įdiegta vartotojo kontekste, sistemos diegimas perrašo įdiegtį vartotojo kontekste.</span><span class="sxs-lookup"><span data-stu-id="d96dc-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="d96dc-107">Jei sistemos kontekste įdiegta "Microsoft Edge", bus pateikta diegimo sėkmė.</span><span class="sxs-lookup"><span data-stu-id="d96dc-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="d96dc-108">Iš anksto įdiegtos "Microsoft Edge" 77 ir vėlesnės versijos visiems vartotojo konteksto kanalams bus perrašyti "Microsoft Edge", įdiegta sistemos kontekste.</span><span class="sxs-lookup"><span data-stu-id="d96dc-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="d96dc-109">**Būtina sąlyga**</span><span class="sxs-lookup"><span data-stu-id="d96dc-109">**Prerequisite**</span></span>

<span data-ttu-id="d96dc-110">"Windows 10" versija 1709 arba vėlesnės versijos</span><span class="sxs-lookup"><span data-stu-id="d96dc-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="d96dc-111">**Veiksmai, kaip įtraukti Edge į Intune**</span><span class="sxs-lookup"><span data-stu-id="d96dc-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="d96dc-112">[Konfigūruokite programą Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="d96dc-113">[Konfigūruokite taikomosios programos informaciją](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="d96dc-114">[Konfigūruokite taikomosios programos parametrus](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="d96dc-115">[Pažymėkite aprėpties žymas (pasirinktinai)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="d96dc-116">[Įtraukite taikomąją programą](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="d96dc-117">Daugiau pagalbos rasite [trikčių diagnostika](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d96dc-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




