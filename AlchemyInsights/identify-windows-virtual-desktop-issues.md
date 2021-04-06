---
title: "\"Windows\" virtualiojo darbalaukio problemų šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595853"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="6cd7e-102">"Windows" virtualiojo darbalaukio problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="6cd7e-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="6cd7e-103">"Windows Virtual Desktop Diagnostics" naudoja tik vieną "PowerShell" "cmdlet", tačiau joje yra daug pasirinktinių parametrų, kurie padeda susiaurinti ir atskirti problemas.</span><span class="sxs-lookup"><span data-stu-id="6cd7e-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="6cd7e-104">Norėdami pradėti:</span><span class="sxs-lookup"><span data-stu-id="6cd7e-104">To get started:</span></span> 

1. <span data-ttu-id="6cd7e-105">Atsisiųskite ir importuokite "Windows Virtual Desktop PowerShell" modulį.</span><span class="sxs-lookup"><span data-stu-id="6cd7e-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="6cd7e-106">Daugiau informacijos žr. ["Windows Virtual Desktop Cmdlet", skirta "Windows PowerShell".](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="6cd7e-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="6cd7e-107">Norėdami prisijungti prie savo paskyros, vykdykite šią "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="6cd7e-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="6cd7e-108">Pavyzdys: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="6cd7e-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="6cd7e-109">**PASTABA:** Visose užklausose, kuriose naudojama "PowerShell", turi būti -UserName arba -ActivityID parametrai.</span><span class="sxs-lookup"><span data-stu-id="6cd7e-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="6cd7e-110">Stebėjimo galimybes žr. [Žurnalo analizės naudojimas diagnostikos funkcijai](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="6cd7e-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="6cd7e-111">Norėdami filtruoti diagnostines veiklas pagal vartotoją, vykdykite šią "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="6cd7e-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="6cd7e-112">Pavyzdys: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="6cd7e-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="6cd7e-113">Yra filtrų, kuriuos galite naudoti problemoms diagnozuoti, sąrašas.</span><span class="sxs-lookup"><span data-stu-id="6cd7e-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="6cd7e-114">Norėdami sužinoti daugiau apie problemų diagnozavimo klausimus, [žr. "Windows" virtualiojo darbalaukio](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)problemų šalinimas ir diagnostika.</span><span class="sxs-lookup"><span data-stu-id="6cd7e-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="6cd7e-115">Norėdami sužinoti daugiau apie įprastas klaidas, [žr. Bendrosios klaidos senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="6cd7e-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
