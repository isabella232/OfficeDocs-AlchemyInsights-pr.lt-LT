---
title: Diegti Office 365 ProPlus bendrai naudoti RDS, terminalo serverio arba VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959467"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="7dba1-102">Diegti Office 365 ProPlus bendrai naudoti RDS, terminalo serverio arba VDI</span><span class="sxs-lookup"><span data-stu-id="7dba1-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="7dba1-103">Norėdami įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos (RDS), anksčiau pavadintas terminalų tarnybos:</span><span class="sxs-lookup"><span data-stu-id="7dba1-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="7dba1-104">Turite turėti "Microsoft 365 for Business" planą arba "Office 365" planą, kuriame yra "Office 365 ProPlus", pvz., "Office 365 Enterprise E3" arba "Enterprise E5".</span><span class="sxs-lookup"><span data-stu-id="7dba1-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="7dba1-105">Office 365 Business "ir" Office 365 "Business Premium" planai neapima "Office 365 ProPlus".</span><span class="sxs-lookup"><span data-stu-id="7dba1-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="7dba1-106">Turite įgalinti [bendrai kompiuterio aktyvinimas](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="7dba1-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="7dba1-107">Taip pat galite atsisiųsti ir paleisti [Microsoft Support ir atkūrimo asistentas](https://aka.ms/SaRA_OfficeSCA_M365Portal) įdiegti Office 365 ProPlus bendrai naudojamo kompiuterio aktyvinimo režimu.</span><span class="sxs-lookup"><span data-stu-id="7dba1-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="7dba1-108">Daugiau informacijos apie Būtinosios sąlygos, sąrankos instrukcijos ir nurodymai dėl individualų įrenginių naudodami Office visuotinio diegimo įrankį, ieškokite [įdiegti Office 365 ProPlus naudojant nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="7dba1-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="7dba1-109">Norėdami ištaisyti klaidas, susijusias su bendrai naudojamo kompiuterio aktyvinimu:</span><span class="sxs-lookup"><span data-stu-id="7dba1-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="7dba1-110">Peržiūrėkite " [Office 365 ProPlus" bendrai naudojamo kompiuterio aktyvinimo problemų triktis](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="7dba1-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="7dba1-111">Peržiūrėkite [iš naujo nustatyti "Office 365 ProPlus" aktyvinimo būseną](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="7dba1-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="7dba1-112">Jei norite įdiegti Office 365 ProPlus RDS iš "Microsoft" 365 administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7dba1-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="7dba1-113">Patikrinkite, ką Office 365 planą turite.</span><span class="sxs-lookup"><span data-stu-id="7dba1-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="7dba1-114">[Sužinokite, kaip](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)tai daryti.</span><span class="sxs-lookup"><span data-stu-id="7dba1-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="7dba1-115">Jei reikia, pereikite į kitą Office 365 planą.</span><span class="sxs-lookup"><span data-stu-id="7dba1-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="7dba1-116">[Sužinokite, kaip](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)tai daryti.</span><span class="sxs-lookup"><span data-stu-id="7dba1-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="7dba1-117">Jei Office jau yra įdiegta RDS serveryje naudojant kitus Office 365 planus, pašalinkite jį.</span><span class="sxs-lookup"><span data-stu-id="7dba1-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="7dba1-118">Pavyzdžiui, eikite į **valdymo skydo** > **išdiegti programą**.</span><span class="sxs-lookup"><span data-stu-id="7dba1-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="7dba1-119">Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei jūs naudojate problemų.</span><span class="sxs-lookup"><span data-stu-id="7dba1-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="7dba1-120">RDS serveryje Prisijunkite prie "Microsoft" 365 administravimo centro su savo administratoriaus abonementu ir [įdiekite "Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)".</span><span class="sxs-lookup"><span data-stu-id="7dba1-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="7dba1-121">Įdiegus "Office", ***neatidarykite arba prisijunkite*** prie jokių "Office" taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="7dba1-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="7dba1-122">RDS serveryje, įgalinti bendrai kompiuterio aktyvinimas redaguodami registrą atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7dba1-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="7dba1-123">Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite **vykdyti**.</span><span class="sxs-lookup"><span data-stu-id="7dba1-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="7dba1-124">Lauke Atidaryti įveskite **regedit**, ir tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="7dba1-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="7dba1-125">Pasirinkite **taip** Kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="7dba1-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="7dba1-126">Registro rengyklėje pridėkite eilutės reikšmę **Sharedcomputerlicensing** su parametr 1 pagal HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="7dba1-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="7dba1-127">RDS serveryje, ***Prisijunkite kaip galutiniam vartotojui*** ir [patikrinkite, ar bendrai kompiuterio aktyvinimas yra įjungtas Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="7dba1-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

