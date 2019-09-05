---
title: Office diegimas terminalų serveryje-nelicencijuotos
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735397"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="af679-102">Office diegimas terminalų serveryje</span><span class="sxs-lookup"><span data-stu-id="af679-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="af679-103">Diegti Office 365 ProPlus Windows Server naudojant nuotolinio darbalaukio tarnybos (RDS), anksčiau pavadintas terminalų tarnybos:</span><span class="sxs-lookup"><span data-stu-id="af679-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="af679-104">Turite turėti Office 365 planą, kuriame yra Office 365 ProPlus, pvz., Office 365 Enterprise E3 arba Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="af679-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="af679-105">Office 365 Business "ir" Office 365 "Business Premium" planai neapima "Office 365 ProPlus".</span><span class="sxs-lookup"><span data-stu-id="af679-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="af679-106">Turite įgalinti [bendrai naudojamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="af679-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="af679-107">Jei norite įdiegti Office 365 ProPlus RDS iš "Microsoft" 365 administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="af679-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="af679-108">Patikrinkite, ką Office 365 planą turite.</span><span class="sxs-lookup"><span data-stu-id="af679-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="af679-109">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="af679-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="af679-110">Jei reikia, pereikite į kitą Office 365 planą.</span><span class="sxs-lookup"><span data-stu-id="af679-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="af679-111">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="af679-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="af679-112">Jei Office jau yra įdiegta RDS serveryje naudojant kitus Office 365 planus, pašalinkite jį.</span><span class="sxs-lookup"><span data-stu-id="af679-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="af679-113">Pvz., eikite į valdymo skydo \> išdiegti programą.</span><span class="sxs-lookup"><span data-stu-id="af679-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="af679-114">Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei jūs naudojate problemų.</span><span class="sxs-lookup"><span data-stu-id="af679-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="af679-115">RDS serveryje Prisijunkite prie "Microsoft" 365 administravimo centro su savo administratoriaus abonementu ir [įdiekite "Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)".</span><span class="sxs-lookup"><span data-stu-id="af679-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="af679-116">Įdiegus "Office", ***neatidarykite arba prisijunkite*** prie jokių "Office" taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="af679-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="af679-117">RDS serveryje, įgalinti bendrai kompiuterio aktyvinimas redaguodami registrą atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="af679-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="af679-118">Apatiniame kairiajame ekrano kampe dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką ir pasirinkite vykdyti.</span><span class="sxs-lookup"><span data-stu-id="af679-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="af679-119">Lauke Atidaryti įveskite **regedit**, ir tada pasirinkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="af679-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="af679-120">Pasirinkite taip, kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="af679-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="af679-121">Registro rengyklėje pridėkite eilutės reikšmę **Sharedcomputerlicensing** su parametr 1 pagal HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="af679-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="af679-122">RDS serveryje, ***Prisijunkite kaip galutiniam vartotojui*** ir [patikrinkite, ar bendrai kompiuterio aktyvinimas yra įjungtas Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="af679-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="af679-123">Daugiau informacijos apie Būtinosios sąlygos, sąrankos instrukcijos ir nurodymai dėl individualų įrenginių naudodami Office visuotinio diegimo įrankį, ieškokite [įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="af679-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="af679-124">Norėdami ištaisyti klaidas, susijusias su bendrai naudojamo kompiuterio aktyvinimu, žiūrėkite [trikčių diagnostika bendrai naudojamame kompiuterio aktyvinimui Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="af679-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  