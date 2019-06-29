---
title: Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353185"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b2d8a-102">Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas</span><span class="sxs-lookup"><span data-stu-id="b2d8a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b2d8a-103">Puslapyje [domenai](https://portal.office.com/adminportal/home#/Domains) domenų, sąraše pažymėkite domeno naudojate savo svetainę, ir tada pasirinkite **DNS parametrus** valdymo srityje.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="b2d8a-104">Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="b2d8a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b2d8a-105">**DNS** tipo įveskite: **(adresas)**</span><span class="sxs-lookup"><span data-stu-id="b2d8a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="b2d8a-106">**Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite:**@**</span><span class="sxs-lookup"><span data-stu-id="b2d8a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="b2d8a-107">**IP adresą**, įveskite statinį IP adresą į savo svetainę, kur ji šiuo metu yra Patalpinta (pavyzdžiui, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="b2d8a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="b2d8a-108">Tai turi būti svetainės, ne *dinaminis* IP adresas yra *statinis* IP adresas.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="b2d8a-109">Teiraukitės svetainę kur jūsų svetainė hosted įsitikinkite, kad jums yra Statinis IP adresas, jūsų viešąją žiniatinklio svetainę.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="b2d8a-110">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-110">Select **Save**.</span></span>

<span data-ttu-id="b2d8a-111">Be to, sukuriate CNAME įrašą, padėti klientams surasti jūsų svetainę.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b2d8a-112">Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="b2d8a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="b2d8a-113">**DNS** tipo įveskite: **CNAME (pseudonimas)**</span><span class="sxs-lookup"><span data-stu-id="b2d8a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="b2d8a-114">**Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite: **www**</span><span class="sxs-lookup"><span data-stu-id="b2d8a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="b2d8a-115">**Atkreipia dėmesį į adresą**, įrašykite visiškai apibrėžtą domeno vardą (FQDN) į savo svetainę (pvz.,.: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b2d8a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="b2d8a-116">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="b2d8a-116">Select **Save**.</span></span>
