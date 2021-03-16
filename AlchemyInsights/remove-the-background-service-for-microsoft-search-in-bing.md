---
title: "\"Microsoft\" ieškos fone paslaugos šalinimas \"Bing\""
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816204"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="3334d-102">"Microsoft" ieškos fone paslaugos šalinimas "Bing"</span><span class="sxs-lookup"><span data-stu-id="3334d-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="3334d-103">Norėdami pašalinti "Microsoft Search" fono paslaugą "Bing", galite išbandyti šias priemones:</span><span class="sxs-lookup"><span data-stu-id="3334d-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="3334d-104">Norėdami atkurti pradinius ieškos modulio parametrus, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="3334d-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="3334d-105">a.</span><span class="sxs-lookup"><span data-stu-id="3334d-105">a.</span></span> <span data-ttu-id="3334d-106">Perjunkite jungiklį **naudoti "Bing" kaip numatytąjį ieškos [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) modulį**.</span><span class="sxs-lookup"><span data-stu-id="3334d-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="3334d-107">b.</span><span class="sxs-lookup"><span data-stu-id="3334d-107">b.</span></span> <span data-ttu-id="3334d-108">[Eikite į "Microsoft" 365 administravimo centrą](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ir išvalykite parametrą, kuris paveikia visus jūsų organizacijos vartotojus.</span><span class="sxs-lookup"><span data-stu-id="3334d-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="3334d-109">Kad pašalintumėte fono paslaugą iš atskiro įrenginio, atlikite šias užduotis:</span><span class="sxs-lookup"><span data-stu-id="3334d-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="3334d-110">a.</span><span class="sxs-lookup"><span data-stu-id="3334d-110">a.</span></span> <span data-ttu-id="3334d-111">Pasirinkite **valdymo skydas > programos > programos ir funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="3334d-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="3334d-112">b.</span><span class="sxs-lookup"><span data-stu-id="3334d-112">b.</span></span> <span data-ttu-id="3334d-113">Dešiniuoju pelės mygtuku spustelėkite **"Microsoft" ieška "Bing** " įdiegtų programų sąraše, tada spustelėkite **pašalinti**.</span><span class="sxs-lookup"><span data-stu-id="3334d-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="3334d-114">Kad pašalintumėte fono paslaugą iš kelių organizacijos įrenginių, registruokitės kaip administratorius ir vykdykite šią komandą dalyje scenarijus:</span><span class="sxs-lookup"><span data-stu-id="3334d-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
