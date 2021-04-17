---
title: ATNAUJINKITE DNS įrašus, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827534"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="bc0b8-102">ATNAUJINKITE DNS įrašus, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju</span><span class="sxs-lookup"><span data-stu-id="bc0b8-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="bc0b8-103">"Microsoft 365" administravimo centre eikite į puslapį Domenų sąranka, o domenų sąraše pasirinkite domeną,  >  [](https://admin.microsoft.com/Adminportal#/Domains) kurį naudojate savo žiniatinklio svetainei.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="bc0b8-104">Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:</span><span class="sxs-lookup"><span data-stu-id="bc0b8-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bc0b8-105">**Jei norite įvesti DNS** tipą: A **(Adresas)**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="bc0b8-106">Jei **tai pagrindinio kompiuterio vardas arba pseudonimas,** įveskite: **@**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="bc0b8-107">**Jei norite naudoti IP** adresą, įveskite statinį svetainės, kurioje jis šiuo metu nuomojamas, IP adresą (pvz., 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="bc0b8-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="bc0b8-108">Tai turi būti  *statinis svetainės*  IP adresas, o ne  *dinaminis*  IP adresas.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="bc0b8-109">Patikrinkite svetainę, kurioje laikoma jūsų svetainė, kad įsitikintumėte, jog galite gauti statinį viešosios žiniatinklio svetainės IP adresą.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="bc0b8-110">Pasirinkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-110">Select **Save**.</span></span>

<span data-ttu-id="bc0b8-111">Be to, galite sukurti CNAME įrašą, kad klientai galėtų rasti jūsų svetainę.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="bc0b8-112">Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:</span><span class="sxs-lookup"><span data-stu-id="bc0b8-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bc0b8-113">**Jei norite įvesti DNS** tipą: **CNAME (pseudonimas)**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="bc0b8-114">Jei **reikia pagrindinio kompiuterio vardo arba pseudonimo,** įveskite: **www**</span><span class="sxs-lookup"><span data-stu-id="bc0b8-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="bc0b8-115">Dalyje **Adreso taškai** įveskite visiškai apibrėžtą savo svetainės domeno vardą (FQDN) (pvz., contoso.com).</span><span class="sxs-lookup"><span data-stu-id="bc0b8-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="bc0b8-116">Pasirinkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="bc0b8-116">Select **Save**.</span></span>
