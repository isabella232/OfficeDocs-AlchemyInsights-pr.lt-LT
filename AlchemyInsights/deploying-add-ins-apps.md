---
title: "\"\"Microsoft 365\" programos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125678"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="928aa-102">""Microsoft 365" programos</span><span class="sxs-lookup"><span data-stu-id="928aa-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="928aa-103">Centralizuotas diegimas yra rekomenduojamas būdas diegti Office papildinių vartotojams ir grupėms jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="928aa-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="928aa-104">Norėdami įdiegti papildiniai, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="928aa-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="928aa-105">**Pastaba:** Norėdami įdiegti papildinių, Office kaip atskiras vartotojas, žr. Papildinių rodymas, valdymas [ir diegimas Office programose.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="928aa-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="928aa-106">Taip pat įsitikinkite, kad įgalintas Office parduotuvės papildinių įsigijimas.</span><span class="sxs-lookup"><span data-stu-id="928aa-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="928aa-107">Įsitikinkite, kad jūsų aplinka atitinka papildinių diegimo naudojant centralizuotą diegimą reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="928aa-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="928aa-108">Daugiau informacijos žr. [Reikalavimai](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="928aa-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="928aa-109">Eikite **Parametrai** Integruotos programos Gaukite programėlių  >    >   Microsoft 365 administravimo centre, kad diegdami papildiniai.</span><span class="sxs-lookup"><span data-stu-id="928aa-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="928aa-110">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="928aa-110">Notes:</span></span> 

- <span data-ttu-id="928aa-111">Integruotos programos reikalauja, kad administratorius turėtų visuotinio administratoriaus arba Exchange administratoriaus teises.</span><span class="sxs-lookup"><span data-stu-id="928aa-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="928aa-112">Kai papildiniai diegiami keliems vartotojams, rekomenduojame užduotis atlikti naudojant grupes, o ne atskirus vartotojus.</span><span class="sxs-lookup"><span data-stu-id="928aa-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="928aa-113">Daugiau informacijos [žr. Papildinių priskyrimo vartotojams ir grupėms aspektai.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="928aa-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="928aa-114">Centralizuotas diegimas nepalaiko vartotojų įdėtosiose grupėse arba grupėse, kurios turi pirmines grupes.</span><span class="sxs-lookup"><span data-stu-id="928aa-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="928aa-115">Daugiau informacijos [žr. Vartotojų ir grupių užduotys](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="928aa-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="928aa-116">Įsitikinkite, kad "Microsoft 365 App Management Service" (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') yra įgalinta vartotojams prisijungti.</span><span class="sxs-lookup"><span data-stu-id="928aa-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="928aa-117">Daugiau informacijos žr. [Taikomosios programos ypatybės konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="928aa-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="928aa-118">Jei kyla problemų diegiant papildinį naudojant integruotas programas, pabandykite įdiegti naudodami [papildinį.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="928aa-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="928aa-119">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="928aa-119">For more information, see:</span></span>

<span data-ttu-id="928aa-120">[Papildiniai diegiami administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Papildiniai administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Centralizuoto diegimo "PowerShell" "cmdlet" naudojimas papildinių valdymas](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publikavimas Office papildiniai naudojant centralizuotą diegimą Microsoft 365 administravimo centre](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Trikčių šalinimas: vartotojas nematote papildiniai](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Vartotojo klaidų šalinimas naudojant Office papildiniai](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="928aa-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>