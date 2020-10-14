---
title: "\"Intune Win32\" taikomųjų programų diegimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461873"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="88b80-102">"Intune Win32" taikomųjų programų diegimas</span><span class="sxs-lookup"><span data-stu-id="88b80-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="88b80-103">"Microsoft Intune" leidžia Win32 taikomąsias programas, įskaitant, bet neapsiribojant, MSI ir. EXE turi būti įdiegtas į "Windows 10" įrenginius.</span><span class="sxs-lookup"><span data-stu-id="88b80-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="88b80-104">Naudojamam diegimo mechanizmui reikalingas Intune Management Extension (IME) paskirties įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="88b80-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="88b80-105">IME bus automatiškai įdiegta kaip "PowerShell" scenarijų arba "Win32" taikomųjų programų diegimas vartotojui/įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="88b80-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="88b80-106">Taip pat yra išankstinių sąlygų, kurios turi būti įvykdytos norint įdiegti Win32 taikomąsias programas, kurios apima:</span><span class="sxs-lookup"><span data-stu-id="88b80-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="88b80-107">Palaikomos platformos: "Windows 10" versija 1607 arba naujesnė ("Enterprise", "Pro" ir "Education" versijos).</span><span class="sxs-lookup"><span data-stu-id="88b80-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="88b80-108">Palaikoma architektūra: x86 ir x64.</span><span class="sxs-lookup"><span data-stu-id="88b80-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="88b80-109">Įrenginių valdymas: AAD sujungtos ir automatiškai užregistruotos (įskaitant hibridinį domeną, sujungtą su grupe ir grupės strategija).</span><span class="sxs-lookup"><span data-stu-id="88b80-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="88b80-110">Taikomosios programos paketo formatas:. **intunewin**  failas, parengtas ["Microsoft Win32" turinio prep įrankyje](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="88b80-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="88b80-111">Apribojimai</span><span class="sxs-lookup"><span data-stu-id="88b80-111">Limitations:</span></span>
    - <span data-ttu-id="88b80-112">Maksimalus dydis: 8GB.</span><span class="sxs-lookup"><span data-stu-id="88b80-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="88b80-113">Nepalaikoma architektūra: ginklai.</span><span class="sxs-lookup"><span data-stu-id="88b80-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="88b80-114">Norėdami gauti informacijos, susijusios su tais veiksmais, peržiūrėkite "[Microsoft Intune" Win32 programos "įtraukti, priskirti ir stebėti](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" dok.</span><span class="sxs-lookup"><span data-stu-id="88b80-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="88b80-115">Išsami informacija apie taikomųjų programų diegimo sistemoje "Windows", įskaitant "Win32" taikomąsias programas, galima peržiūrėti šiuose dokumentuose</span><span class="sxs-lookup"><span data-stu-id="88b80-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="88b80-116">Taikomųjų programų diegimo problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="88b80-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="88b80-117">"Win32" taikomųjų programų trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="88b80-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)