---
title: Biuro diegimas terminalų serveryje - Nelicencijuota
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763225"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="cb3a6-102">"Office" diegimas terminalų serveryje</span><span class="sxs-lookup"><span data-stu-id="cb3a6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="cb3a6-103">Microsoft 365 programėlių įmonėms diegti "Windows Server" naudojant nuotolinio darbalaukio tarnybas (RDS), anksčiau vadintą terminalų tarnybomis:</span><span class="sxs-lookup"><span data-stu-id="cb3a6-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="cb3a6-104">Turite turėti "Microsoft 365" prenumeratą, kurioje yra "Microsoft 365" programos verslui, pvz., "Office 365 Enterprise E3" arba "Enterprise E5".</span><span class="sxs-lookup"><span data-stu-id="cb3a6-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="cb3a6-105">"Microsoft 365" programos verslui ir "Microsoft 365" programos verslui "Premium" planuose neapima "Microsoft 365" programėlių įmonėms.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="cb3a6-106">Turite įjungti [bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="cb3a6-107">Jei norite įdiegti "Microsoft 365 Apps" įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite šiuos veiksmus.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="cb3a6-108">Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo asistentas](https://aka.ms/SaRA_OfficeSCA_M365Portal) įdiegti "Microsoft 365 Apps" įmonėms bendro naudojimo kompiuterio aktyvinimo režimu.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="cb3a6-109">Patikrinkite, ką turite "Microsoft 365" prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="cb3a6-110">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="cb3a6-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="cb3a6-111">Jei reikia, perjunkite į kitą "Microsoft 365" prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="cb3a6-112">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="cb3a6-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="cb3a6-113">Jei "Office" jau įdiegtas RDS serveryje naudojant kitas "Microsoft 365" prenumeratas, pašalinkite ją.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="cb3a6-114">Pavyzdžiui, eikite į \> Valdymo skydas Pašalinti programą.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="cb3a6-115">Pašalinkite naudodami ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei kyla problemų.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="cb3a6-116">RDS serveryje prisijunkite prie "Microsoft 365" administravimo centro naudodami administratoriaus abonementą ir [įdiekite "Microsoft 365 Apps for enterprise".](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="cb3a6-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="cb3a6-117">Įdiegę "Office", ***neatidarykite ir neprisijunkite prie*** jokių "Office" taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="cb3a6-118">RDS serveryje, įgalinti bendro naudojimo kompiuterio aktyvinimo redaguodami registrą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="cb3a6-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="cb3a6-119">Dešiniuoju pelės mygtuku spustelėkite mygtuką "Windows", esantį apatiniame kairiajame ekrano kampe, ir pasirinkite Vykdyti.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="cb3a6-120">Lauke Atidaryti įveskite **regedit**, tada pasirinkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="cb3a6-121">Pasirinkite Taip, kai būsite paraginti leisti registro rengyklę keisti jūsų įrenginį.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="cb3a6-122">Registro rengyklėje įtraukite **SharedComputerLicensing** eilutės reikšmę su parametru 1, esantį HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="cb3a6-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="cb3a6-123">RDS ***serveryje, prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar bendrai naudojamas kompiuterio aktyvinimas yra įjungtas Microsoft 365 Apps verslui](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="cb3a6-124">Daugiau informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir rekomendacijas dėl tinkintų diegimų naudojant "Office" diegimo įrankį rasite ["Microsoft 365" programėlių diegimas įmonei naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="cb3a6-125">Norėdami ištaisyti klaidas, susijusias su kompiuterio aktyvinimu, peržiūrėkite [Trikčių šalinimas naudojant bendrai naudojamą kompiuterio aktyvinimą, skirtą "Microsoft 365" programėlėms, skirtai įmonei](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="cb3a6-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  