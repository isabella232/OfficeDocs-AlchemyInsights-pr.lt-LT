---
title: Offboard ne "Windows" įrenginiai iš "Microsoft Defender" išplėstinės grėsmės apsauga (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748476"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="9f3d9-102">Offboard ne "Windows" įrenginiai iš "Microsoft Defender" išplėstinės grėsmės apsauga (ATP)</span><span class="sxs-lookup"><span data-stu-id="9f3d9-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="9f3d9-103">Toliau nurodyta, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-103">Here's how:</span></span>

1. <span data-ttu-id="9f3d9-104">Vykdykite trečiosios šalies dokumentus, kad atjungtumėte trečiosios šalies sprendimą iš "Microsoft Defender ATP".</span><span class="sxs-lookup"><span data-stu-id="9f3d9-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="9f3d9-105">Naudodami "Azure Active Directory" nuomotoją, pašalinkite trečiosios šalies sprendimo teises:</span><span class="sxs-lookup"><span data-stu-id="9f3d9-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="9f3d9-106">Prisijunkite prie " [Azure" portalo](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="9f3d9-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="9f3d9-107">Pasirinkite **Visos tarnybos**"  >  **Azure Active Directory**  >  **Enterprise" taikomosios programos**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="9f3d9-108">Pasirinkite taikomąją programą, kurią norite atlikti.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="9f3d9-109">Pasirinkite **Naikinti**.</span><span class="sxs-lookup"><span data-stu-id="9f3d9-109">Select **Delete**.</span></span>

<span data-ttu-id="9f3d9-110">Jei norite sužinoti daugiau, skaitykite [ne "Windows" įrenginių offboard](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="9f3d9-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
