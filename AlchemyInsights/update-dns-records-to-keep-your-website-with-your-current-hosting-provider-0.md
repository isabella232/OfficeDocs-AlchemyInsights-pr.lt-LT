---
title: Atnaujinkite DNS įrašus, kad jūsų svetainė būtų išsaugota su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665768"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="a755b-102">Atnaujinkite DNS įrašus, kad jūsų svetainė būtų išsaugota su dabartiniu išteklių nuomos teikėju</span><span class="sxs-lookup"><span data-stu-id="a755b-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="a755b-103">"Microsoft 365" administravimo centre eikite į puslapį **Sąrankos**  >  [domenai](https://portal.office.com/adminportal/home#/Domains) ir domenų sąraše pasirinkite domeną, kurį naudojate savo svetainei.</span><span class="sxs-lookup"><span data-stu-id="a755b-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="a755b-104">Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:</span><span class="sxs-lookup"><span data-stu-id="a755b-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a755b-105">**DNS tipui** įveskite: **A (adresas)**</span><span class="sxs-lookup"><span data-stu-id="a755b-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="a755b-106">Pagrindinio **kompiuterio vardą arba pseudonimą**įveskite:**@**</span><span class="sxs-lookup"><span data-stu-id="a755b-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="a755b-107">**IP adresui**įveskite svetainės, kurioje šiuo metu nuomojama, statinį IP adresą (pvz., 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="a755b-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="a755b-108">Tai turi būti *statinis* IP adresas svetainėje, o ne *dinaminis* IP adresas.</span><span class="sxs-lookup"><span data-stu-id="a755b-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="a755b-109">Pasitarkite su svetaine, kurioje nuomojama jūsų svetainė, kad įsitikintumėte, jog galite gauti statinį viešosios žiniatinklio svetainės IP adresą.</span><span class="sxs-lookup"><span data-stu-id="a755b-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="a755b-110">Pasirinkite **I¹saugoti**.</span><span class="sxs-lookup"><span data-stu-id="a755b-110">Select **Save**.</span></span>

<span data-ttu-id="a755b-111">Be to, galite sukurti CNAME įrašą, kad padėtumėte klientams rasti jūsų svetainę.</span><span class="sxs-lookup"><span data-stu-id="a755b-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="a755b-112">Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:</span><span class="sxs-lookup"><span data-stu-id="a755b-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a755b-113">**DNS tipui** įveskite: **CNAME (pseudonimas)**</span><span class="sxs-lookup"><span data-stu-id="a755b-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="a755b-114">Pagrindinio **kompiuterio vardą arba pseudonimą**įveskite: **www**</span><span class="sxs-lookup"><span data-stu-id="a755b-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="a755b-115">Jei **norite, kad nukreipia adresu**, įveskite visiškai apibrėžtą domeno vardą (FQDN) savo svetainei (pvz., contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a755b-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="a755b-116">Pasirinkite **I¹saugoti**.</span><span class="sxs-lookup"><span data-stu-id="a755b-116">Select **Save**.</span></span>
