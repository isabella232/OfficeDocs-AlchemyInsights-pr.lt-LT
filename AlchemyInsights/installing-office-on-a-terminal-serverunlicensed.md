---
title: "\"Office\" diegimas terminalo serveryje – nelicencijuotas"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663125"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f276b-102">"Office" diegimas terminalo serveryje</span><span class="sxs-lookup"><span data-stu-id="f276b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f276b-103">Diegiant "Microsoft" 365 taikomąsias programas įmonėms "Windows Server", naudojant nuotolinio darbalaukio tarnybas (RDS), anksčiau pavadintas terminalų tarnybos:</span><span class="sxs-lookup"><span data-stu-id="f276b-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f276b-104">Turite turėti "Microsoft" 365 prenumeratą, kuri aprėpia "Microsoft 365" taikomąsias programas įmonėms, pvz., "Office 365 Enterprise E3" arba "Enterprise E5".</span><span class="sxs-lookup"><span data-stu-id="f276b-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="f276b-105">"Microsoft" 365 taikomosios programos verslui ir "Microsoft 365" verslui priemokų planams neapima "Microsoft 365" taikomųjų programų įmonėms.</span><span class="sxs-lookup"><span data-stu-id="f276b-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="f276b-106">Reikia įjungti [bendrinamą kompiuterio aktyvinimą](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="f276b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="f276b-107">Jei norite įdiegti "Microsoft" 365 taikomąsias programas įmonėms RDS iš "Microsoft 365" administravimo centro, ***kuris naudoja numatytuosius diegimo parametrus***, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="f276b-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="f276b-108">Taip pat galite atsisiųsti ir paleisti ["Microsoft" palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA_OfficeSCA_M365Portal) , kad įdiegtumėte "microsoft" 365 taikomąsias programas, skirtas įmonės bendrinamo kompiuterio aktyvinimo režimu.</span><span class="sxs-lookup"><span data-stu-id="f276b-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="f276b-109">Patikrinkite, kokią "Microsoft" 365 prenumeratą turite.</span><span class="sxs-lookup"><span data-stu-id="f276b-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="f276b-110">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="f276b-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="f276b-111">Jei reikia, perjunkite kitą "Microsoft" 365 prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="f276b-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="f276b-112">Sužinokite, kaip</span><span class="sxs-lookup"><span data-stu-id="f276b-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="f276b-113">Jei "Office" jau yra įdiegtas RDS serveryje naudodami kitas "Microsoft 365" prenumeratas, pašalinkite ją.</span><span class="sxs-lookup"><span data-stu-id="f276b-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="f276b-114">Pvz., nuėję į valdymo skydo \> pašalinti programą.</span><span class="sxs-lookup"><span data-stu-id="f276b-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="f276b-115">Pašalinkite ["Microsoft" palaikymo ir atkūrimo pagalbinė priemonė,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jei naudojate problemas.</span><span class="sxs-lookup"><span data-stu-id="f276b-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="f276b-116">RDS serveryje Prisijunkite prie "Microsoft 365" administravimo centro naudodami savo administratoriaus abonementą ir [įdiekite "microsoft 365" taikomąsias programas, skirtas įmonėms](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="f276b-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="f276b-117">Įdiegę "Office", ***neatidarykite arba prisijunkite*** prie bet kurios "Office" taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="f276b-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="f276b-118">RDS serveryje įjunkite bendrinamą kompiuterio aktyvinimą redaguodami registrą atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="f276b-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="f276b-119">Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką apatiniame kairiajame ekrano kampe ir pasirinkite vykdyti.</span><span class="sxs-lookup"><span data-stu-id="f276b-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="f276b-120">Lauke Atidaryti įveskite **regedit**, tada pasirinkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="f276b-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="f276b-121">Pasirinkite taip, kai būsite paraginti leisti registro rengyklę atlikti jūsų įrenginio keitimą.</span><span class="sxs-lookup"><span data-stu-id="f276b-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="f276b-122">Registro rengyklėje įtraukite " **Sharedcomputerlicensing** " eilutės reikšmę su 1 parametru HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="f276b-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="f276b-123">RDS serveryje ***Prisijunkite kaip galutinis vartotojas*** ir [patikrinkite, ar įgalintas bendrinamas kompiuterio aktyvinimas "Microsoft" "365" programoms, skirtos įmonėms](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="f276b-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="f276b-124">Išsamesnės informacijos apie būtinąsias sąlygas, sąrankos instrukcijas ir patarimus apie tinkintus diegimus naudojant "Office" diegimo įrankį, žr. ["Microsoft 365" taikomųjų programų diegimas įmonėms naudojant nuotolinio darbalaukio tarnybas](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="f276b-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="f276b-125">Norėdami ištaisyti klaidas, susijusias su bendrinamo kompiuterio aktyvinimu, peržiūrėkite triktis, susijusias [su bendrinamo kompiuterio aktyvinimu "Microsoft" 365 programoms Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="f276b-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  