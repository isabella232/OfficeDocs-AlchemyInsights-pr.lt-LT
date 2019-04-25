---
title: Diegti "office" Terminal Server - be leidimų
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410130"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="a94a7-102">Diegti "Office" terminalo serverio</span><span class="sxs-lookup"><span data-stu-id="a94a7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="a94a7-103">Diegiant "Office 365 ProPlus" naudodami nuotolinio darbalaukio tarnybų (RDS) Windows Server, vadintas terminalų tarnybos:</span><span class="sxs-lookup"><span data-stu-id="a94a7-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="a94a7-104">Turite "Office 365" planą, kuris apima "Office 365 ProPlus", pvz., Office 365 Enterprise E3 "arba" Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="a94a7-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="a94a7-105">Office 365 Business "ir" Office 365 Business Premium planus neįeina "Office 365 ProPlus".</span><span class="sxs-lookup"><span data-stu-id="a94a7-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="a94a7-106">Jums reikia įgalinti [bendrinamo kompiuterio suaktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="a94a7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="a94a7-107">Jei norite įdiegti "Office 365 ProPlus" RDS "Office 365" portale \*\* *kuri naudoja numatytąjį diegimo parametrus* \*\*, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a94a7-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="a94a7-108">Patikrinkite, ką turite "Office 365" planą.</span><span class="sxs-lookup"><span data-stu-id="a94a7-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="a94a7-109">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="a94a7-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="a94a7-110">Jei reikia, pereiti prie skirtingų "Office 365" planą.</span><span class="sxs-lookup"><span data-stu-id="a94a7-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="a94a7-111">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="a94a7-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="a94a7-112">Jei Office yra įdiegta RDS serverio naudojant kitus "Office 365" planus, pašalinkite ją.</span><span class="sxs-lookup"><span data-stu-id="a94a7-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="a94a7-113">Pvz., nuėję į valdymo skydo \> pašalinti programą.</span><span class="sxs-lookup"><span data-stu-id="a94a7-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="a94a7-114">Pašalinti, jei kyla problemų naudojant ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="a94a7-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="a94a7-115">RDS serveriu, prisijunkite prie "Office 365" portale su administratoriaus paskyrą ir [įdiegti "Office 365 ProPlus"](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="a94a7-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="a94a7-116">Po to, kai Office yra įdiegta, \*\* *ne atidaryti arba prisijunkite* \*\* į visas Office programas.</span><span class="sxs-lookup"><span data-stu-id="a94a7-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="a94a7-117">RDS serverio, kad aktyvinimo bendrai naudojamame kompiuteryje iš registro redagavimą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a94a7-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="a94a7-118">Dešiniuoju pelės mygtuku spustelėkite apatiniame kairiajame kampe ekrano "Windows" mygtuką ir pasirinkite paleisti.</span><span class="sxs-lookup"><span data-stu-id="a94a7-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="a94a7-119">Lauke Atidaryti įveskite **regedit**, ir pasirinkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="a94a7-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="a94a7-120">Pasirinkite taip, kai būsite paprašyti leisti registro redaktorių keisti įrenginio.</span><span class="sxs-lookup"><span data-stu-id="a94a7-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="a94a7-121">Registro redaktoriaus, pridėti eilutės reikšmė, **SharedComputerLicensing** 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, kuriame.</span><span class="sxs-lookup"><span data-stu-id="a94a7-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="a94a7-122">RDS serverio, \*\* *kaip galutinio vartotojo Prisijunkite* \*\* ir [patikrinkite aktyvinimo bendrai naudojamame kompiuteryje įgalintas, "Office 365 ProPlus"](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="a94a7-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="a94a7-123">Daugiau informacijos apie būtinųjų sąlygų, sąrankos nurodymus ir patarimus individualų įrenginių naudodami Office diegimo įrankis, žiūrėkite [Diegti Office 365 ProPlus naudodami nuotolinio darbalaukio tarnybos](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="a94a7-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="a94a7-124">Ištaisyti klaidas, susijusias su bendra kompiuterio aktyvinimu, žiūrėkite [trikčių problemas aktyvinamą bendrai naudojamame kompiuteryje, "Office 365 ProPlus"](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="a94a7-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

