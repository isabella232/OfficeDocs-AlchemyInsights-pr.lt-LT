---
title: Esamo monitoriaus trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738576"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="714bd-102">Esamo monitoriaus trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="714bd-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="714bd-103">Išbandykite šiuos sprendimus monitoriui šalinti.</span><span class="sxs-lookup"><span data-stu-id="714bd-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="714bd-104">**Atnaujinkite monitoriaus ekraną:**</span><span class="sxs-lookup"><span data-stu-id="714bd-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="714bd-105">Vienu metu paspauskite šiuos klavišus: "Windows" klavišas + "Ctrl" + "Shift" + B. Taip bus atnaujintas ryšys su grafikos tvarkykle.</span><span class="sxs-lookup"><span data-stu-id="714bd-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="714bd-106">Jūsų monitoriai mirksės trumpam ir po kelių sekundžių grįš.</span><span class="sxs-lookup"><span data-stu-id="714bd-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="714bd-107">**Monitoriaus aparatūros trikčių diagnostika:**</span><span class="sxs-lookup"><span data-stu-id="714bd-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="714bd-108">Atjunkite kabelį, jungiančio kompiuterį prie monitoriaus, ir vėl jį prijunkite.</span><span class="sxs-lookup"><span data-stu-id="714bd-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="714bd-109">Atjunkite visus neesminius prietaisus iš savo kompiuterio (pvz., adapterius arba dokus).</span><span class="sxs-lookup"><span data-stu-id="714bd-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="714bd-110">**Jei neseniai įdiegėte naujinimą savo kompiuteryje, galite atkurti ekrano tvarkyklę:**</span><span class="sxs-lookup"><span data-stu-id="714bd-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="714bd-111">Pasirinkite **pradėti**, įveskite **įrenginių tvarkytuvė**ir rezultatuose pasirinkite **įrenginių tvarkytuvė** .</span><span class="sxs-lookup"><span data-stu-id="714bd-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="714bd-112">Išplėskite skyrių **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite ekrano plokštę, tada pasirinkite **Ypatybės**.</span><span class="sxs-lookup"><span data-stu-id="714bd-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="714bd-113">Pereikite į skirtuką **tvarkyklė** ir pasirinkite **Atšaukti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="714bd-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="714bd-114">Pastaba: jei tai nepasiekiama arba yra papilkinti, pasirinkite **ne** iš toliau pateiktų parinkčių, kad pereitumėte prie kito veiksmo.</span><span class="sxs-lookup"><span data-stu-id="714bd-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="714bd-115">Gali reikėti iš naujo paleisti kompiuterį, kad įsigaliotų šie keitimai.</span><span class="sxs-lookup"><span data-stu-id="714bd-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="714bd-116">**Pašalinkite ir iš naujo įdiekite ekrano tvarkyklę:**</span><span class="sxs-lookup"><span data-stu-id="714bd-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="714bd-117">Pasirinkite **pradėti**, įveskite **įrenginių tvarkytuvė**ir rezultatuose pasirinkite **įrenginių tvarkytuvė** .</span><span class="sxs-lookup"><span data-stu-id="714bd-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="714bd-118">Išplėskite skyrių **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite ekrano adapterį, tada pasirinkite **pašalinti įrenginį**.</span><span class="sxs-lookup"><span data-stu-id="714bd-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="714bd-119">Pažymėkite laukelį šalia **panaikinti šio įrenginio tvarkyklės programinę įrangą** ir pasirinkite **pašalinti**.</span><span class="sxs-lookup"><span data-stu-id="714bd-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="714bd-120">Pastaba: šiame etape jūsų gali būti paprašyta paleisti kompiuterį iš naujo.</span><span class="sxs-lookup"><span data-stu-id="714bd-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="714bd-121">Prieš paleisdami iš naujo Būtinai užsirašykite likusias instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="714bd-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="714bd-122">Dar kartą atidarykite įrenginių tvarkytuvę.</span><span class="sxs-lookup"><span data-stu-id="714bd-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="714bd-123">Išplėskite skyrių **rodymo adapteriai** , dešiniuoju pelės mygtuku spustelėkite ekrano adapterį ir pasirinkite **Naujinti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="714bd-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="714bd-124">Pasirinkite **automatiškai ieškoti tvarkyklės programinės įrangos** ir vykdykite diegimo instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="714bd-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>