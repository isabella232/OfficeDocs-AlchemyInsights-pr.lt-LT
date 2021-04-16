---
title: "\"Bluetooth\" problemų sprendimas sistemoje \"Windows 10\""
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812940"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="a9cd8-102">"Bluetooth" problemų sprendimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="a9cd8-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="a9cd8-103">Jei nėra "Bluetooth" piktogramos arba "Bluetooth" negalima įjungti arba išjungti, galbūt norėsite paleisti "Bluetooth" trikčių diagnostikos priemonę.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="a9cd8-104">[Atidarykite parametrų trikčių](ms-settings:troubleshoot)diagnostiką , dalyje **Rasti ir** išspręsti kitas problemas spustelėkite **"Bluetooth",** spustelėkite **Paleisti trikčių diagnostikos priemonę**.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="a9cd8-105">Jei nematote "Bluetooth" piktogramos, bet "Bluetooth" rodoma įrenginių tvarkytuvėje:</span><span class="sxs-lookup"><span data-stu-id="a9cd8-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="a9cd8-106">Įrenginių tvarkytuvėje spustelėkite **"Bluetooth".**</span><span class="sxs-lookup"><span data-stu-id="a9cd8-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="a9cd8-107">Paspauskite ir laikykite (arba dešiniuoju pelės mygtuku spustelėkite) "Bluetooth" adapterio pavadinimą ir spustelėkite **Pašalinti įrenginį.**</span><span class="sxs-lookup"><span data-stu-id="a9cd8-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="a9cd8-108">Išjunkite "Windows" įrenginį, palaukite kelias sekundes, tada vėl jį įjunkite.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="a9cd8-109">"Windows" bandys iš naujo įdiegti tvarkyklę.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="a9cd8-110">Jei neseniai įdiegėte "Windows 10" naujinimus arba atnaujinote versiją į "Windows 10", galbūt norėsite patikrinti, ar yra tvarkyklės naujinimų:</span><span class="sxs-lookup"><span data-stu-id="a9cd8-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="a9cd8-111">Įrenginių tvarkytuvėje spustelėkite **"Bluetooth",** tada spustelėkite "Bluetooth" adapterio pavadinimą (kuriame gali būti žodis "radijas").</span><span class="sxs-lookup"><span data-stu-id="a9cd8-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="a9cd8-112">Paspauskite ir laikykite (arba dešiniuoju pelės mygtuku spustelėkite) "Bluetooth" adapterį, tada spustelėkite Naujinti  >  **tvarkyklę Automatiškai ieškoti atnaujintos tvarkyklės programinės įrangos.**</span><span class="sxs-lookup"><span data-stu-id="a9cd8-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="a9cd8-113">Atlikite veiksmus, tada spustelėkite **Uždaryti**.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="a9cd8-114">Jei "Windows" negali rasti naujos "Bluetooth" tvarkyklės, apsilankykite kompiuterio gamintojo svetainėje ir atsisiųskite naujausią "Bluetooth" tvarkyklę iš ten.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="a9cd8-115">Atsisiuntę, spustelėkite **Naujinti** tvarkyklę Naršykite mano kompiuteryje tvarkyklės programinę įrangą Ieškokite vietos, kurioje saugomi  >    >  tvarkyklės failai, > **Gerai** Pirmyn ir atlikite diegimo  >  veiksmus.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="a9cd8-116">Įdiegę atnaujintą tvarkyklę, iš naujo paleiskite kompiuterį ir patikrinkite, ar tai išsprendžia ryšio problemą.</span><span class="sxs-lookup"><span data-stu-id="a9cd8-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="a9cd8-117">Daugiau informacijos, kaip šalinti "Bluetooth" problemas, žr. visą straipsnį ["Bluetooth" problemų sprendimas sistemoje "Windows 10".](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="a9cd8-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
