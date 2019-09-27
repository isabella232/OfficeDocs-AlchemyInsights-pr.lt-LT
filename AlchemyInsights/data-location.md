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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207269"
---
# <a name="data-location"></a><span data-ttu-id="7c319-102">Duomenų vieta</span><span class="sxs-lookup"><span data-stu-id="7c319-102">Data location</span></span>

<span data-ttu-id="7c319-103">Galite peržiūrėti savo "Office 365" nuomotojo vietą administravimo centre arba prisijungti prie "Exchange Online" per "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="7c319-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="7c319-104">**Administravimo centras:**</span><span class="sxs-lookup"><span data-stu-id="7c319-104">**Admin center:**</span></span>
1. <span data-ttu-id="7c319-105">Prisijunkite prie [administravimo centro](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="7c319-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="7c319-106">Pasirinkite **Parametrai** > **organizacijos profilis**.</span><span class="sxs-lookup"><span data-stu-id="7c319-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="7c319-107">Dalyje **duomenų vieta**pasirinkite **Peržiūrėti išsamią informaciją**.</span><span class="sxs-lookup"><span data-stu-id="7c319-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="7c319-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="7c319-108">**PowerShell:**</span></span>
1. <span data-ttu-id="7c319-109">Prisijungti prie Exchange Online naudojant "Windows PowerShell".</span><span class="sxs-lookup"><span data-stu-id="7c319-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="7c319-110">Vykdyti [gauti-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet Rodyti savo nuomotojo ypatybes sąrašą.</span><span class="sxs-lookup"><span data-stu-id="7c319-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="7c319-111">Peržiūrėkite ypatybę OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="7c319-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="7c319-112">Jei turite EXO ir SPO duomenų vietą, galite nustatyti duomenų vietą kitoms paslaugoms, kurias galite naudoti iš [ten, kur yra jūsų duomenys](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="7c319-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>