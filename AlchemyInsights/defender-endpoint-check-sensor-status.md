---
title: Sargybos pabaigos taško tikrinimo jutiklio būsena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676343"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="969c6-102">Sargybos pabaigos taško tikrinimo jutiklio būsena</span><span class="sxs-lookup"><span data-stu-id="969c6-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="969c6-103">Plytelė **Įrenginiai su jutiklio** problemomis yra saugos operacijų ataskaitų srityje.</span><span class="sxs-lookup"><span data-stu-id="969c6-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="969c6-104">Šioje plytelėje pateikiama informacija apie atskiro įrenginio galimybę pateikti jutiklio duomenis ir bendrauti su galinio punkto tarnybos sargyba.</span><span class="sxs-lookup"><span data-stu-id="969c6-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="969c6-105">Ji praneša, kiek įrenginių reikia atkreipti dėmesį ir padeda nustatyti probleminius įrenginius ir imtis veiksmų, kad būtų išsekusi žinomos problemos.</span><span class="sxs-lookup"><span data-stu-id="969c6-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="969c6-106">Du plytelės būsenos indikatoriai pateikia informaciją apie įrenginių, kurie netinkamai praneša tarnybai, skaičių:</span><span class="sxs-lookup"><span data-stu-id="969c6-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="969c6-107">**Netinkamai sukonfigūruota** Įrenginiai, kurie gali iš dalies pranešti jutiklio duomenis galinio punkto tarnybos sargybai ir gali turėti konfigūracijos klaidų, kurias reikia ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="969c6-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="969c6-108">**Neaktyvus** Įrenginiai, kurie nustojo teikti ataskaitas galinio punkto tarnybos sargybai daugiau nei septynias dienas per pastarąjį mėnesį.</span><span class="sxs-lookup"><span data-stu-id="969c6-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="969c6-109">Spustelėjus bet kurią iš grupių, nukreipiama į sąrašą Įrenginiai, filtruojamas pagal jūsų pasirinkimus.</span><span class="sxs-lookup"><span data-stu-id="969c6-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="969c6-110">Sąraše Įrenginiai galite filtruoti sveikatos būsenų sąrašą pagal šią būseną:</span><span class="sxs-lookup"><span data-stu-id="969c6-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="969c6-111">**Aktyvus** Įrenginiai, kurie aktyviai praneša pabaigos taško tarnybos sargybai.</span><span class="sxs-lookup"><span data-stu-id="969c6-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="969c6-112">**Netinkamai sukonfigūruota** Įrenginiai, kurie gali iš dalies pranešti jutiklio duomenis galinio punkto tarnybos sargybai, tačiau turi konfigūracijos klaidų, kurias reikia ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="969c6-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="969c6-113">Netinkamai sukonfigūruotuose įrenginiuose gali būti viena iš šių problemų arba jų derinys:</span><span class="sxs-lookup"><span data-stu-id="969c6-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="969c6-114">Nėra jutiklio duomenų – įrenginiai nustojo siųsti jutiklio duomenis.</span><span class="sxs-lookup"><span data-stu-id="969c6-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="969c6-115">Iš įrenginio gali būti paleidžiami riboti įspėjimai.</span><span class="sxs-lookup"><span data-stu-id="969c6-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="969c6-116">Sutrikę ryšiai – galimybė bendrauti su įrenginiu yra sutrikusi.</span><span class="sxs-lookup"><span data-stu-id="969c6-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="969c6-117">Failų siuntimas giliai analizei, failų blokavimas, įrenginio izoliavimas nuo tinklo ir kiti veiksmai, kuriems reikia ryšio su įrenginiu, gali neveikti.</span><span class="sxs-lookup"><span data-stu-id="969c6-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="969c6-118">**Neaktyvus** Įrenginiai, kurie nustojo teikti ataskaitas galinių punktų tarnybos sargybai.</span><span class="sxs-lookup"><span data-stu-id="969c6-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="969c6-119">Galite atsisiųsti visą sąrašą CSV formatu naudodami eksportavimo funkciją.</span><span class="sxs-lookup"><span data-stu-id="969c6-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="969c6-120">Daugiau informacijos žr. Jutiklio [sveikatos būsenos tikrinimas "Microsoft" sargybos galinį punktą](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="969c6-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="969c6-121">Daugiau informacijos apie tai, dėl ko įrenginys buvo neaktyvus arba netinkamai sukonfigūruotas, žr. Nesveikų jutiklių taisymas ["Microsoft Defender", skirtame galinių punktų .](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="969c6-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
