---
title: Duomenų vieta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655290"
---
# <a name="data-location"></a><span data-ttu-id="063d1-102">Duomenų vieta</span><span class="sxs-lookup"><span data-stu-id="063d1-102">Data location</span></span>

<span data-ttu-id="063d1-103">Galite peržiūrėti savo nuomotojo vietą administravimo centre arba prisijungę prie "Exchange Online" per "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="063d1-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="063d1-104">**Administravimo centras:**</span><span class="sxs-lookup"><span data-stu-id="063d1-104">**Admin center:**</span></span>
1. <span data-ttu-id="063d1-105">Prisijunkite prie [administravimo centro](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="063d1-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="063d1-106">Pasirinkite **Parametrai** > **Organizacijos profilis**.</span><span class="sxs-lookup"><span data-stu-id="063d1-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="063d1-107">Dalyje **Duomenų vieta**pasirinkite **Peržiūrėti išsamią informaciją**.</span><span class="sxs-lookup"><span data-stu-id="063d1-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="063d1-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="063d1-108">**PowerShell:**</span></span>
1. <span data-ttu-id="063d1-109">Prisijunkite prie "Exchange Online" naudodami "Windows PowerShell".</span><span class="sxs-lookup"><span data-stu-id="063d1-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="063d1-110">Vykdykite [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet, kad būtų rodomas nuomotojo ypatybių sąrašas.</span><span class="sxs-lookup"><span data-stu-id="063d1-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="063d1-111">Pažvelkite į OrganizationId ypatybę.</span><span class="sxs-lookup"><span data-stu-id="063d1-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="063d1-112">Jei turite EXO ir SPO duomenų vietą, galite nustatyti kitų paslaugų, kurias galite [naudoti, duomenų](https://products.office.com/where-is-your-data-located)vietą iš Kur yra jūsų duomenys .</span><span class="sxs-lookup"><span data-stu-id="063d1-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>