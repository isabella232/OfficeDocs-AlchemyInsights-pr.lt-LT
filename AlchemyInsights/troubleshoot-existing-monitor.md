---
title: Esamo monitoriaus trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824587"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="98135-102">Esamo monitoriaus trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="98135-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="98135-103">Išbandykite šiuos monitorių trikčių šalinimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="98135-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="98135-104">**Atnaujinkite monitoriaus ekraną:**</span><span class="sxs-lookup"><span data-stu-id="98135-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="98135-105">Vienu metu paspauskite šiuos klavišus: "Windows" klavišas + "Ctrl" + "Shift" + B. Taip atnaujinsite ryšį su grafikos tvarkykle.</span><span class="sxs-lookup"><span data-stu-id="98135-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="98135-106">Jūsų monitoriai mirksės iš karto ir grįš po kelių sekundžių.</span><span class="sxs-lookup"><span data-stu-id="98135-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="98135-107">**Monitoriaus aparatūros trikčių šalinimas:**</span><span class="sxs-lookup"><span data-stu-id="98135-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="98135-108">Atjunkite kabelį, jungiantį kompiuterį su monitoriu, ir vėl jį prijunkite.</span><span class="sxs-lookup"><span data-stu-id="98135-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="98135-109">Atjunkite visus neesmines priemones iš kompiuterio (pvz., adapterių ar dokų).</span><span class="sxs-lookup"><span data-stu-id="98135-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="98135-110">**Jei neseniai įdiegėte naujinimą kompiuteryje, galite atšaukti ekrano tvarkyklę:**</span><span class="sxs-lookup"><span data-stu-id="98135-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="98135-111">Pasirinkite **Pradžia**, įveskite **įrenginių tvarkytuvė** ir **rezultatuose pasirinkite** Įrenginių tvarkytuvė.</span><span class="sxs-lookup"><span data-stu-id="98135-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="98135-112">Išplėskite **sekciją Rodymo adapteriai,** dešiniuoju pelės mygtuku spustelėkite rodymo adapterį ir pasirinkite **Ypatybės**.</span><span class="sxs-lookup"><span data-stu-id="98135-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="98135-113">Eikite į **skirtuką Tvarkyklė** ir pasirinkite **Atšaukti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="98135-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="98135-114">Pastaba: jei ši parinktis negalima arba yra pilka, pasirinkite **Ne** iš toliau pateikiamų parinkčių, kad pereidami prie kito veiksmo.</span><span class="sxs-lookup"><span data-stu-id="98135-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="98135-115">Prieš įsigaliojant šiems pokyčiams, gali tekti iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="98135-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="98135-116">**Pašalinkite ir iš naujo įdiekite rodymo tvarkyklę:**</span><span class="sxs-lookup"><span data-stu-id="98135-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="98135-117">Pasirinkite **Pradžia**, įveskite **įrenginių tvarkytuvė** ir **rezultatuose pasirinkite** Įrenginių tvarkytuvė.</span><span class="sxs-lookup"><span data-stu-id="98135-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="98135-118">Išplėskite **sekciją Rodymo adapteriai,** dešiniuoju pelės mygtuku spustelėkite rodymo adapterį ir pasirinkite **Pašalinti įrenginį.**</span><span class="sxs-lookup"><span data-stu-id="98135-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="98135-119">Pažymėkite laukelį šalia Naikinti **šio įrenginio tvarkyklės programinę įrangą ir** pasirinkite **Pašalinti**.</span><span class="sxs-lookup"><span data-stu-id="98135-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="98135-120">Pastaba: šiame etape jūsų gali paprašyti iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="98135-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="98135-121">Prieš paleisdami iš naujo, būtinai užsirašykite likusias instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="98135-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="98135-122">Dar kartą atidarykite įrenginių tvarkytuvę.</span><span class="sxs-lookup"><span data-stu-id="98135-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="98135-123">Išplėskite **sekciją Rodymo adapteriai,** dešiniuoju pelės mygtuku spustelėkite rodymo adapterį ir pasirinkite **Naujinti tvarkyklę**.</span><span class="sxs-lookup"><span data-stu-id="98135-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="98135-124">Pasirinkite **Automatiškai ieškoti tvarkyklės programinės įrangos naujinimo ir** vykdykite diegimo instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="98135-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>