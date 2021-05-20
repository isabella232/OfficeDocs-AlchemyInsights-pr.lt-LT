---
title: Problemos, susijusios su už borto arba išjungto įrenginio pašalinimu iš įrenginio atsargų
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564342"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="79000-102">Problemos, susijusios su už borto arba išjungto įrenginio pašalinimu iš įrenginio atsargų</span><span class="sxs-lookup"><span data-stu-id="79000-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="79000-103">"Microsoft" pabaigos taško sargyba šiuo metu neleidžia rankiniu būdu pašalinti įrenginio, išjungto arba išjungto įrenginio, įrašo iš įrenginio atsargų.</span><span class="sxs-lookup"><span data-stu-id="79000-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="79000-104">Saugumo sumetimais įrenginys lieka portale kaip istorinis įrašas iki 180 dienų.</span><span class="sxs-lookup"><span data-stu-id="79000-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="79000-105">Tačiau įrenginio duomenys išvalomi pagal sukonfigūruotą saugojimo laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="79000-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="79000-106">**Pastaba:** Išjungto arba išjungto įrenginio būsena po septynių dienų **automatiškai** persijungia į neaktyvią būseną.</span><span class="sxs-lookup"><span data-stu-id="79000-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="79000-107">Be to, įrenginiai, kurie nėra aktyvūs per paskutines 30 dienų, nėra įtraukti į duomenis, kurie atspindi jūsų organizaciją grėsmių ir pažeidžiamumų valdymas arba "Microsoft Secure Score for Devices".</span><span class="sxs-lookup"><span data-stu-id="79000-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="79000-108">Jei vis tiek nenorite matyti tam tikrų įrenginių rodinyje Įrenginių atsargos, pabandykite pateikti įrenginio žymę, kad išfiltruosite išjungtą įrenginį rodinyje Įrenginio atsargos.</span><span class="sxs-lookup"><span data-stu-id="79000-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="79000-109">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="79000-109">For more information, see:</span></span>

[<span data-ttu-id="79000-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="79000-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="79000-111">Poveikio balas grėsmių ir pažeidžiamumų valdymas</span><span class="sxs-lookup"><span data-stu-id="79000-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="79000-112">Nesveikų jutiklių taisymas "Microsoft Defender", skirtame "Endpoint"</span><span class="sxs-lookup"><span data-stu-id="79000-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="79000-113">Kaip efektyviai naudoti žymėjimą (1 dalis)</span><span class="sxs-lookup"><span data-stu-id="79000-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="79000-114">Kaip efektyviai naudoti žymėjimą (2 dalis)</span><span class="sxs-lookup"><span data-stu-id="79000-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="79000-115">Kaip efektyviai naudoti žymėjimą (3 dalis)</span><span class="sxs-lookup"><span data-stu-id="79000-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




