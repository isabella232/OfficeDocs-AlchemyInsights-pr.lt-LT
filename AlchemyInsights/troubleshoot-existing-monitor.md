---
title: Trikčių diagnostika esamas monitorius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690719"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="1dcc4-102">Esamo monitoriaus trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="1dcc4-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="1dcc4-103">Išbandykite šiuos sprendimus, kad išspręstumėte monitorių.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="1dcc4-104">**Atnaujinkite monitoriaus rodymą:**</span><span class="sxs-lookup"><span data-stu-id="1dcc4-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="1dcc4-105">Vienu metu paspauskite šiuos klavišus: "Windows" klavišas + "Ctrl" + "Shift" + B. Taip bus atnaujintas ryšys su jūsų grafikos tvarkykle.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="1dcc4-106">Jūsų monitoriai mirksės akimirksniu ir grįš po kelių sekundžių.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="1dcc4-107">**Monitoriaus aparatūros trikčių diagnostika:**</span><span class="sxs-lookup"><span data-stu-id="1dcc4-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="1dcc4-108">Atjunkite kabelį, jungiantį kompiuterį su monitoriumi, ir vėl jį prijunkite.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="1dcc4-109">Atjunkite visus neesminius savo kompiuterio įrenginius (pvz., adapterius arba dokus).</span><span class="sxs-lookup"><span data-stu-id="1dcc4-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="1dcc4-110">**Jei neseniai įdiegėte naujinimą kompiuteryje, galite atšaukti savo rodymo tvarkyklę:**</span><span class="sxs-lookup"><span data-stu-id="1dcc4-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="1dcc4-111">Pasirinkite **Pradžia**, įveskite **Device Manager**ir pasirinkite **įrenginių tvarkytuvas** iš rezultatų.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1dcc4-112">Išplėskite sekciją **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite savo rodymo adapterį, ands pasirinkite **Properties (ypatybės**).</span><span class="sxs-lookup"><span data-stu-id="1dcc4-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="1dcc4-113">Pereikite į skirtuką **tvarkyklė** ir pasirinkite **Atšaukti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="1dcc4-114">Pastaba: jei tai nėra arba yra papilkinta, pasirinkite **ne** iš toliau pateiktų parinkčių, kad pereitumėte prie paskesnio veiksmo.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="1dcc4-115">Gali tekti iš naujo paleisti kompiuterį, kad įsigaliotų šie pokyčiai.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="1dcc4-116">**Ekrano tvarkyklės šalinimas ir diegimas iš naujo:**</span><span class="sxs-lookup"><span data-stu-id="1dcc4-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="1dcc4-117">Pasirinkite **Pradžia**, įveskite **Device Manager**ir pasirinkite **įrenginių tvarkytuvas** iš rezultatų.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1dcc4-118">Išplėskite sekciją **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite ekrano adapterį, ands pasirinkite **pašalinti įrenginį**.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="1dcc4-119">Pažymėkite žymės langelį, esantį prie **panaikinti šio įrenginio tvarkyklės programinę įrangą** , ir pasirinkite **pašalinti**.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="1dcc4-120">Pastaba: šiame etape gali būti paprašyta iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="1dcc4-121">Prieš paleisdami iš naujo Būtinai užsirašykite likusias instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="1dcc4-122">Dar kartą atidarykite įrenginių tvarkytuvę.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="1dcc4-123">Išplėskite sekciją **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite ekrano adapterį ir pasirinkite **Naujinti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="1dcc4-124">**Norėdami atnaujinti tvarkyklės programinę įrangą, pasirinkite Ieškoti automatiškai** ir vykdykite diegimo instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="1dcc4-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>