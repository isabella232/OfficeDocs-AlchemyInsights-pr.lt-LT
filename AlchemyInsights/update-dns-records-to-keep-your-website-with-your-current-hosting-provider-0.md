---
title: Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480552"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="f1b9c-102">Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas</span><span class="sxs-lookup"><span data-stu-id="f1b9c-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="f1b9c-103">Puslapyje [domenai](https://portal.office.com/adminportal/home#/Domains) domenų, sąraše pažymėkite domeno naudojate savo svetainę, ir tada pasirinkite **DNS parametrus** valdymo srityje.</span><span class="sxs-lookup"><span data-stu-id="f1b9c-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="f1b9c-104">Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="f1b9c-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="f1b9c-105">**DNS** tipo įveskite: **(adresas)**</span><span class="sxs-lookup"><span data-stu-id="f1b9c-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="f1b9c-106">**Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite:**@**</span><span class="sxs-lookup"><span data-stu-id="f1b9c-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="f1b9c-107">**IP adresą**, įveskite statinį IP adresą į savo svetainę, kur ji šiuo metu yra Patalpinta (pavyzdžiui, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="f1b9c-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="f1b9c-p101">Tai turi būti svetainės, ne *dinaminis* IP adresas yra *statinis* IP adresas. Teiraukitės svetainę kur jūsų svetainė hosted įsitikinkite, kad jums yra Statinis IP adresas, jūsų viešąją žiniatinklio svetainę.</span><span class="sxs-lookup"><span data-stu-id="f1b9c-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="f1b9c-110">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="f1b9c-110">Select **Save**.</span></span> 
    
<span data-ttu-id="f1b9c-111">Be to, sukuriate CNAME įrašą, padėti klientams surasti jūsų svetainę.</span><span class="sxs-lookup"><span data-stu-id="f1b9c-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="f1b9c-112">Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="f1b9c-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="f1b9c-113">**DNS** tipo įveskite: **CNAME (pseudonimas)**</span><span class="sxs-lookup"><span data-stu-id="f1b9c-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="f1b9c-114">**Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite: **www**</span><span class="sxs-lookup"><span data-stu-id="f1b9c-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="f1b9c-115">**Atkreipia dėmesį į adresą**, įrašykite visiškai apibrėžtą domeno vardą (FQDN) į savo svetainę (pvz.,.: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f1b9c-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="f1b9c-116">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="f1b9c-116">Select **Save**.</span></span> 
    

