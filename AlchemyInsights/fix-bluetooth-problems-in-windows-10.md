---
title: "\"Bluetooth\" problemų sprendimas sistemoje \"Windows 10\""
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730167"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="31693-102">"Bluetooth" problemų sprendimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="31693-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="31693-103">Jei nėra "Bluetooth" piktogramos arba "Bluetooth" negalima įjungti arba išjungti, galbūt norėsite paleisti "Bluetooth" trikčių diagnostikos priemonę.</span><span class="sxs-lookup"><span data-stu-id="31693-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="31693-104">[Atidarykite trikčių diagnostikos parametrus](ms-settings:troubleshoot), spustelėkite **"Bluetooth"** dalyje **radimas ir Išspręskite kitas problemas**, spustelėkite **paleisti trikčių diagnostikos priemonę**.</span><span class="sxs-lookup"><span data-stu-id="31693-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="31693-105">Jei nematote "Bluetooth" piktogramos, bet "Bluetooth" rodoma įrenginių tvarkytuvėje:</span><span class="sxs-lookup"><span data-stu-id="31693-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="31693-106">Įrenginių tvarkytuvėje spustelėkite **"Bluetooth"**.</span><span class="sxs-lookup"><span data-stu-id="31693-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="31693-107">Paspauskite ir laikykite (arba spustelėkite dešiniuoju pelės mygtuku) "Bluetooth" adapterio pavadinimą ir spustelėkite **pašalinti įrenginį**.</span><span class="sxs-lookup"><span data-stu-id="31693-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="31693-108">Išjunkite "Windows" įrenginį, palaukite kelias sekundes, tada vėl jį įjunkite.</span><span class="sxs-lookup"><span data-stu-id="31693-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="31693-109">"Windows" bandys iš naujo įdiegti tvarkyklę.</span><span class="sxs-lookup"><span data-stu-id="31693-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="31693-110">Jei neseniai įdiegėte "Windows 10" naujinimus arba atnaujinote į "Windows 10", galbūt norėsite patikrinti, ar yra tvarkyklių naujinimų:</span><span class="sxs-lookup"><span data-stu-id="31693-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="31693-111">Įrenginių tvarkytuvėje spustelėkite **"Bluetooth**", tada spustelėkite "Bluetooth" adapterio pavadinimą (kuris gali apimti žodį "radijas").</span><span class="sxs-lookup"><span data-stu-id="31693-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="31693-112">Paspauskite ir laikykite (arba spustelėkite dešiniuoju pelės mygtuku) "Bluetooth" adapterį ir spustelėkite **Naujinti tvarkyklės**  >  **iešką, kad atnaujintų tvarkyklės programinę įrangą**.</span><span class="sxs-lookup"><span data-stu-id="31693-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="31693-113">Atlikite nurodytus veiksmus, tada spustelėkite **uždaryti**.</span><span class="sxs-lookup"><span data-stu-id="31693-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="31693-114">Jei "Windows" neranda naujos "Bluetooth" tvarkyklės, apsilankykite kompiuterio gamintojo svetainėje ir iš ten Atsisiųskite naujausią "Bluetooth" tvarkyklę.</span><span class="sxs-lookup"><span data-stu-id="31693-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="31693-115">Atsisiuntę spustelėkite **Naujinti tvarkyklę**  >  **mano kompiuteryje ieškoti tvarkyklės programinės įrangos**–  >  **raskite** vietą, kurioje saugomi tvarkyklės failai > **gerai**  >  **toliau**, tada atlikite veiksmus, kuriuos norite įdiegti.</span><span class="sxs-lookup"><span data-stu-id="31693-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="31693-116">Įdiegę atnaujintą tvarkyklę, iš naujo paleiskite kompiuterį, tada patikrinkite, ar tai išsprendžia prisijungimo problemą.</span><span class="sxs-lookup"><span data-stu-id="31693-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="31693-117">Daugiau informacijos apie tai, kaip šalinti "Bluetooth" triktis, rasite išsamiam straipsniui, ["Windows 10" "Bluetooth" problemoms](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)spręsti.</span><span class="sxs-lookup"><span data-stu-id="31693-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
