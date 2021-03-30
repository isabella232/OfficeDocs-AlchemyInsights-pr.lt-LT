---
title: Pagalba nustatant nakties šviesos rodymo parametrą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404666"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="2b08e-102">Pagalba nustatant nakties šviesos rodymo parametrą</span><span class="sxs-lookup"><span data-stu-id="2b08e-102">Help with the night light display setting</span></span>

<span data-ttu-id="2b08e-103">Norėdami sužinoti daugiau apie nakties rodymo parametrus, žr. Nakties laiko nustatymas [sistemoje "Windows 10".](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="2b08e-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="2b08e-104">Jei nakties šviesos parinktys yra pilkos dalyje Parametrai, patikrinkite ekrano tvarkyklę:</span><span class="sxs-lookup"><span data-stu-id="2b08e-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="2b08e-105">Spustelėkite užduočių juostos ieškos lauką ir įveskite **Įrenginių tvarkytuvė**, tada ieškos rezultatuose **pasirinkite** Įrenginių tvarkytuvė.</span><span class="sxs-lookup"><span data-stu-id="2b08e-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="2b08e-106">Išplėskite **Rodymo adapteriai**.</span><span class="sxs-lookup"><span data-stu-id="2b08e-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="2b08e-107">Deja, nakties šviesos funkcija negalima, jei jūsų įrenginys naudoja "DisplayLink" tvarkyklę arba bazinę rodymo tvarkyklę.</span><span class="sxs-lookup"><span data-stu-id="2b08e-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="2b08e-108">Nakties šviesos funkcija naudoja naujausias grafikos technologijas, todėl gali tekti atnaujinti ekrano tvarkyklę:</span><span class="sxs-lookup"><span data-stu-id="2b08e-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="2b08e-109">Patikrinkite, ar yra naujinimų, nueikite **į Pradžia**  >  **Parametrai**  >  **Naujinimas &**  >  **"Windows Update"**  >  **patikrinkite, ar yra naujinimų.**</span><span class="sxs-lookup"><span data-stu-id="2b08e-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="2b08e-110">ARBA</span><span class="sxs-lookup"><span data-stu-id="2b08e-110">OR</span></span>

- <span data-ttu-id="2b08e-111">Apsilankykite aparatūros gamintojo palaikymo svetainėje, kad rankiniu būdu atsisiųstumėte ir įdiegtumėte naujausias rodymo tvarkykles.</span><span class="sxs-lookup"><span data-stu-id="2b08e-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="2b08e-112">Iš naujo nustatykite nakties šviesą registre</span><span class="sxs-lookup"><span data-stu-id="2b08e-112">Reset night light in the registry</span></span>

<span data-ttu-id="2b08e-113">Jei atnaujinus ekrano tvarkyklę nepavyko, gali tekti iš naujo nustatyti nakties šviesą registre.</span><span class="sxs-lookup"><span data-stu-id="2b08e-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="2b08e-114">**Dėmesio:** Šis trikčių šalinimo veiksmas rekomenduojamas tik pažengusiems vartotojams.</span><span class="sxs-lookup"><span data-stu-id="2b08e-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="2b08e-115">Jei netinkamai modifikuojate registrą, gali kilti rimtų problemų.</span><span class="sxs-lookup"><span data-stu-id="2b08e-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="2b08e-116">Jei reikia papildomos apsaugos, prieš modifikuodami registrą sukurkite atsarginę jo kopiją, kad galėsite jį atkurti, jei kyla problemų.</span><span class="sxs-lookup"><span data-stu-id="2b08e-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="2b08e-117">Ieškos lauke įveskite **regedit**, tada ieškos rezultatuose **pasirinkite** Registro rengyklė.</span><span class="sxs-lookup"><span data-stu-id="2b08e-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="2b08e-118">Eikite į šį registro raktą:</span><span class="sxs-lookup"><span data-stu-id="2b08e-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="2b08e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="2b08e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="2b08e-120">Eksportuokite ir panaikinkite šį dalinį raktą:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="2b08e-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="2b08e-121">Eksportuokite ir panaikinkite šį dalinį raktą:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="2b08e-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="2b08e-122">Iš naujo paleiskite "Windows" ir patikrinkite, ar yra nakties šviesos parinkčių.</span><span class="sxs-lookup"><span data-stu-id="2b08e-122">Restart Windows and verify if the night light options are available.</span></span>


