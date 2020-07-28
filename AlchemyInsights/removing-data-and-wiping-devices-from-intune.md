---
title: Duomenų ir valymo įrenginių šalinimas iš "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439645"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="28151-102">Duomenų ir valymo įrenginių šalinimas iš "Intune"</span><span class="sxs-lookup"><span data-stu-id="28151-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="28151-103">Įrenginio išėjimo į pensiją ir įrenginio ištrynimo nuotoliniai veiksmai gali būti naudojami pašalinti "Intune" valdomus įmonės duomenis arba atlikti gamyklinius nustatymus ir grąžinti įrenginio numatytuosius parametrus.</span><span class="sxs-lookup"><span data-stu-id="28151-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="28151-104">Prisijunkite prie "Microsoft 365" įrenginių valdymo ir eikite į **Įrenginiai**  >  **visi įrenginiai**.</span><span class="sxs-lookup"><span data-stu-id="28151-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="28151-105">Pasirinkite įrenginį, kurį norite ištrinti.</span><span class="sxs-lookup"><span data-stu-id="28151-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="28151-106">Pasirinkite nuotolinio ištrynimo tipą, kurį norite atlikti.</span><span class="sxs-lookup"><span data-stu-id="28151-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="28151-107">Išeinant į pensiją ištrina tik organizacinę informaciją, o visi servetėlės atkurti įrenginio gamyklinius nustatymus.</span><span class="sxs-lookup"><span data-stu-id="28151-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="28151-108">Pasirinkite **Taip,** kad patvirtintumėte.</span><span class="sxs-lookup"><span data-stu-id="28151-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="28151-109">Kol valymas bus baigtas, įrenginio veiksmo būsena rodoma kaip Laukiama.</span><span class="sxs-lookup"><span data-stu-id="28151-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="28151-110">Kai veiksmas bus baigtas, valdomo įrenginio sąraše mobiliojo įrenginio nebematysite.</span><span class="sxs-lookup"><span data-stu-id="28151-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="28151-111">**Pastaba** Įmonės duomenų negalima pašalinti iš įrenginių, prijungtų prie "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="28151-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="28151-112">Išsamią informaciją apie veiksmų "Išeiti į pensiją ir ištrynimas" poveikį, įskaitant tai, kas išlaikoma ir kas ištrinama, rasite [Įrenginių šalinimas naudojant ištrynimą, išeikite į pensiją arba rankiniu būdu išpakuodami įrenginį](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="28151-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="28151-113">Norėdami ištrinti visus duomenis iš "macOS" įrenginio, [žr.](https://docs.microsoft.com/intune/device-erase)</span><span class="sxs-lookup"><span data-stu-id="28151-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>