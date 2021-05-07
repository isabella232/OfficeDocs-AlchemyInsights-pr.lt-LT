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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233542"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="4cd3a-102">""Microsoft 365" programos</span><span class="sxs-lookup"><span data-stu-id="4cd3a-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="4cd3a-103">Centralizuotas diegimas yra rekomenduojamas būdas diegti Office papildinių vartotojams ir grupėms jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="4cd3a-104">Norėdami įdiegti papildiniai, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="4cd3a-105">**Pastaba:** Norėdami įdiegti papildinių, Office kaip atskiras vartotojas, žr. Papildinių rodymas, valdymas [ir diegimas Office programose.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="4cd3a-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="4cd3a-106">Taip pat įsitikinkite, kad įgalintas Office parduotuvės papildinių įsigijimas.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="4cd3a-107">Daugiau informacijos [žr. Priedų atsisiuntimų išjungimas](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)išjungus "Office" parduotuvę visuose klientuose (išskyrus Outlook) .</span><span class="sxs-lookup"><span data-stu-id="4cd3a-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="4cd3a-108">Įsitikinkite, kad jūsų aplinka atitinka papildinių diegimo naudojant centralizuotą diegimą reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="4cd3a-109">Daugiau informacijos žr. [Reikalavimai](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="4cd3a-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="4cd3a-110">Eikite **Parametrai** Integruotos programos Gaukite programėlių  >    >   Microsoft 365 administravimo centre, kad diegdami papildiniai.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="4cd3a-111">Pastabos:</span><span class="sxs-lookup"><span data-stu-id="4cd3a-111">Notes:</span></span> 

- <span data-ttu-id="4cd3a-112">Integruotos programos reikalauja, kad administratorius turėtų visuotinio administratoriaus arba Exchange administratoriaus teises.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="4cd3a-113">Kai papildiniai diegiami keliems vartotojams, rekomenduojame užduotis atlikti naudojant grupes, o ne atskirus vartotojus.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="4cd3a-114">Daugiau informacijos [žr. Papildinių priskyrimo vartotojams ir grupėms aspektai.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="4cd3a-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="4cd3a-115">Centralizuotas diegimas nepalaiko vartotojų įdėtosiose grupėse arba grupėse, kurios turi pirmines grupes.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="4cd3a-116">Daugiau informacijos [žr. Vartotojų ir grupių užduotys](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="4cd3a-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="4cd3a-117">Įsitikinkite, kad "Microsoft 365 App Management Service" (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') yra įgalinta vartotojams prisijungti.</span><span class="sxs-lookup"><span data-stu-id="4cd3a-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="4cd3a-118">Daugiau informacijos žr. [Taikomosios programos ypatybės konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="4cd3a-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="4cd3a-119">Jei kyla problemų diegiant papildinį naudojant integruotas programas, pabandykite įdiegti naudodami [papildinį.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="4cd3a-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="4cd3a-120">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="4cd3a-120">For more information, see:</span></span>

<span data-ttu-id="4cd3a-121">[Papildiniai diegiami administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Papildiniai administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Centralizuoto diegimo "PowerShell" "cmdlet" naudojimas papildinių valdymas](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publikavimas Office papildiniai naudojant centralizuotą diegimą Microsoft 365 administravimo centre](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Trikčių šalinimas: vartotojas nematote papildiniai](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Vartotojo klaidų šalinimas naudojant Office papildiniai](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="4cd3a-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>