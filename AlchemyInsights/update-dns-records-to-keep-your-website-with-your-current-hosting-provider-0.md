---
title: Atnaujinkite DNS įrašus ir atnaujinkite savo svetainę su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699527"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="23880-102">Atnaujinkite DNS įrašus ir atnaujinkite savo svetainę su dabartiniu išteklių nuomos teikėju</span><span class="sxs-lookup"><span data-stu-id="23880-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="23880-103">"Microsoft 365" administravimo centre eikite į puslapį **sąrankos**  >  [domenai](https://portal.office.com/adminportal/home#/Domains) ir domenų sąraše pasirinkite domeną, kurį naudojate savo žiniatinklio svetainei.</span><span class="sxs-lookup"><span data-stu-id="23880-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="23880-104">Pasirinkite **+ naujas tinkintas įrašas** ir įrašykite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="23880-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="23880-105">**DNS tipas** įveskite: **a (adresas)**</span><span class="sxs-lookup"><span data-stu-id="23880-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="23880-106">Jei esate **pagrindinio kompiuterio vardas arba pseudonimas**, įveskite: **@**</span><span class="sxs-lookup"><span data-stu-id="23880-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="23880-107">Jei naudojate **IP adresą**, įveskite savo žiniatinklio svetainės, kurioje yra šiuo metu Patalpinta, STATINĮ IP adresą (pvz.,: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="23880-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="23880-108">Tai turi būti  *statinis*  IP adresas žiniatinklio svetainei, o ne  *dinaminis*  IP adresas.</span><span class="sxs-lookup"><span data-stu-id="23880-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="23880-109">Patikrinkite svetainę, kurioje yra jūsų žiniatinklio svetainė, kad įsitikintumėte, jog galite gauti viešosios žiniatinklio svetainės statinį IP adresą.</span><span class="sxs-lookup"><span data-stu-id="23880-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="23880-110">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="23880-110">Select **Save**.</span></span>

<span data-ttu-id="23880-111">Be to, galite sukurti CNAME įrašą, padėsiantį klientams rasti jūsų svetainę.</span><span class="sxs-lookup"><span data-stu-id="23880-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="23880-112">Pasirinkite **+ naujas tinkintas įrašas** ir įrašykite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="23880-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="23880-113">**DNS tipas** įveskite: **CNAME (pseudonimas)**</span><span class="sxs-lookup"><span data-stu-id="23880-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="23880-114">Jei esate **pagrindinio kompiuterio vardas arba pseudonimas**, įveskite: **www**</span><span class="sxs-lookup"><span data-stu-id="23880-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="23880-115">Jei **norite, kad būtų rodomas adresas**, įveskite savo žiniatinklio svetainės visiškai apibrėžtą domeno vardą (FQDN) (pvz., contoso.com).</span><span class="sxs-lookup"><span data-stu-id="23880-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="23880-116">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="23880-116">Select **Save**.</span></span>
