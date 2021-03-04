---
title: Duomenų šalinimas ir įrenginių duomenų ištrynimas iš „Intune“
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416321"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="3d29a-102">Duomenų šalinimas ir įrenginių duomenų ištrynimas iš „Intune“</span><span class="sxs-lookup"><span data-stu-id="3d29a-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="3d29a-103">Norint pašalinti įmonės duomenis, valdomus „Intune“, arba atkurti gamyklinius parametrus ir grąžinti įrenginio numatytuosius parametrus, galima naudoti nuotolinius veiksmus Nustoti naudoti įrenginį ir Įrenginio duomenų ištrynimas.</span><span class="sxs-lookup"><span data-stu-id="3d29a-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="3d29a-104">Prisijunkite prie ataskaitų srities „Microsoft 365“ įrenginių valdymas ir eikite į sritį **Įrenginiai,** > **Visi įrenginiai**.</span><span class="sxs-lookup"><span data-stu-id="3d29a-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="3d29a-105">Pasirinkite įrenginį, kurio duomenis norite ištrinti.</span><span class="sxs-lookup"><span data-stu-id="3d29a-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="3d29a-106">Pasirinkite norimo atlikti nuotolinio ištrynimo tipą.</span><span class="sxs-lookup"><span data-stu-id="3d29a-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="3d29a-107">Funkcija Nustoti naudoti panaikina tik organizacijos informaciją, o tuo tarpu visiškas duomenų ištrynimas atkuria įrenginio gamyklinius parametrus.</span><span class="sxs-lookup"><span data-stu-id="3d29a-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="3d29a-108">Patvirtinkite pasirinkdami **Taip**.</span><span class="sxs-lookup"><span data-stu-id="3d29a-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="3d29a-109">Iki tol, kol ištrynimo veiksmas bus baigtas, įrenginio veiksmo būsena bus rodoma kaip *Laukiama, kol bus nustota naudoti*.</span><span class="sxs-lookup"><span data-stu-id="3d29a-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="3d29a-110">Atlikus veiksmą, mobiliojo įrenginio nebematysite valdomųjų įrenginių sąraše.</span><span class="sxs-lookup"><span data-stu-id="3d29a-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="3d29a-111">Įmonės duomenų negalima pašalinti iš įrenginių, PRIJUNGTŲ prie „Microsoft Azure AD“.</span><span class="sxs-lookup"><span data-stu-id="3d29a-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="3d29a-112">Visą išsamią informaciją apie veiksmų Nustoti naudoti ir Duomenų ištrynimas poveikį, įskaitant tai, kas paliekama ir kas panaikinama, žr. šiuose dokumentuose:</span><span class="sxs-lookup"><span data-stu-id="3d29a-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="3d29a-113">[Įrenginių pašalinimas naudojant duomenų ištrynimo ir nustojimo naudoti funkcijas arba rankiniu būdu išregistruojant įrenginį](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="3d29a-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="3d29a-114">Kaip iš „Intune“ valdomų programų ištrinti tik įmonės duomenis</span><span class="sxs-lookup"><span data-stu-id="3d29a-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="3d29a-115">[Visų duomenų ištrynimas iš „MacOS“ įrenginio](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="3d29a-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>