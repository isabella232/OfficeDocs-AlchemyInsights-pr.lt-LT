---
title: Atlaisvinkite vietos diske sistemoje "Windows 10"
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036590"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a3e60-102">Atlaisvinkite vietos diske sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="a3e60-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a3e60-103">Štai dvi parinktys, kaip atlaisvinti vietos diske sistemoje "Windows":</span><span class="sxs-lookup"><span data-stu-id="a3e60-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a3e60-104">Atlaisvinkite vietos diske sistemoje "Windows 10".</span><span class="sxs-lookup"><span data-stu-id="a3e60-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a3e60-105">Atlaisvinkite vietos "Windows 10" naujinimams su išoriniu saugyklos įrenginiu.</span><span class="sxs-lookup"><span data-stu-id="a3e60-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a3e60-106">Jei po disko valymo vis dar liko vietos diske, gali būti, kad jūsų aplankas temp greitai užpildo programos (. Appx) failus, kuriuos naudoja "Microsoft Store".</span><span class="sxs-lookup"><span data-stu-id="a3e60-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a3e60-107">Norėdami išspręsti šią problemą, iš naujo nustatykite parduotuvę, išvalykite saugyklos talpyklą, tada paleiskite "Windows Update" trikčių diagnostikos priemonę.</span><span class="sxs-lookup"><span data-stu-id="a3e60-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a3e60-108">Prieš tęsdami veiksmus, įsitikinkite, kad "Microsoft" parduotuvės uždaryta.</span><span class="sxs-lookup"><span data-stu-id="a3e60-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a3e60-109">**1 veiksmas: iš naujo nustatykite "Microsoft Store"**</span><span class="sxs-lookup"><span data-stu-id="a3e60-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a3e60-110">**Pastaba** Tai visam laikui panaikina programos duomenis įrenginyje, įskaitant nuostatas ir prisijungimo duomenis.</span><span class="sxs-lookup"><span data-stu-id="a3e60-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a3e60-111">Pasirinkite **pradėti**  >  **Parametrai**  >  **programėlių** programėlės  >  **& funkcijas**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a3e60-112">Programėlių sąraše raskite ir pasirinkite "Microsoft Store".</span><span class="sxs-lookup"><span data-stu-id="a3e60-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a3e60-113">Pasirinkite **Išplėstinės parinktys**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a3e60-114">Slinkite žemyn ir pasirinkite **nustatyti iš naujo**, tada **patvirtinkite iš naujo**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a3e60-115">**2 veiksmas: išvalykite "Microsoft Store" talpyklą**</span><span class="sxs-lookup"><span data-stu-id="a3e60-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a3e60-116">Paspauskite "Windows" logotipo klavišą + R, kad atidarytumėte dialogo langą vykdyti.</span><span class="sxs-lookup"><span data-stu-id="a3e60-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a3e60-117">Įveskite wsreset.exe ir pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a3e60-118">Atidaromas langas tuščia Komandinė eilutė.</span><span class="sxs-lookup"><span data-stu-id="a3e60-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a3e60-119">Po maždaug 10 sekundžių langas užsidaro, o saugykla atidaroma automatiškai.</span><span class="sxs-lookup"><span data-stu-id="a3e60-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a3e60-120">**3 veiksmas: "Windows Update" nustatymas iš naujo**</span><span class="sxs-lookup"><span data-stu-id="a3e60-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a3e60-121">Pasirinkite **pradėti**  >  **Parametrai**  >  **Naujinti & saugos**  >  **trikčių šalinimas**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a3e60-122">Slinkite žemyn ir pasirinkite **"Windows Update"** iš sąrašo ir pasirinkite **paleisti trikčių diagnostikos priemonę**.</span><span class="sxs-lookup"><span data-stu-id="a3e60-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a3e60-123">Iš naujo paleiskite kompiuterį ir patikrinkite, ar vis dar susiduriate su problema.</span><span class="sxs-lookup"><span data-stu-id="a3e60-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

