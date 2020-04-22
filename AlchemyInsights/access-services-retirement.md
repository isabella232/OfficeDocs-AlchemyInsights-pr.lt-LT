---
title: Prieigos prie išėjimo į pensiją paslaugos
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687266"
---
# <a name="access-services-retirement"></a><span data-ttu-id="aa96f-102">Prieigos prie išėjimo į pensiją paslaugos</span><span class="sxs-lookup"><span data-stu-id="aa96f-102">Access services retirement</span></span>

<span data-ttu-id="aa96f-103">Kaip mes iš pradžių paskelbė MC97576, kovo 2017, ir toliau bendrauti per pastaruosius metus Access Services yra pensininkas.</span><span class="sxs-lookup"><span data-stu-id="aa96f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="aa96f-104">Kitas šio proceso etapas bus "Access" žiniatinklio duomenų bazių, naudojančių SharePoint sąrašus kaip pagrindinę duomenų saugyklą, pašalinimas.</span><span class="sxs-lookup"><span data-stu-id="aa96f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="aa96f-105">**Kaip tai veikia mane?**</span><span class="sxs-lookup"><span data-stu-id="aa96f-105">**How does this affect me?**</span></span>

<span data-ttu-id="aa96f-106">Nuo 2019 m. birželio mes nustosime kurti naujas "Access" duomenų bazes "SharePoint Online" ir iki 2020 m. balandžio mėn.</span><span class="sxs-lookup"><span data-stu-id="aa96f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="aa96f-107">**Ką turiu daryti, kad pasiruoščiau šiam pakeitimui?**</span><span class="sxs-lookup"><span data-stu-id="aa96f-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="aa96f-108">Rekomenduojame sukurti perėjimo planą savo organizacijos "Access" žiniatinklio duomenų bazėms.</span><span class="sxs-lookup"><span data-stu-id="aa96f-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="aa96f-109">Administratoriai gali naudoti ["SharePoint Access" taikomųjų programų skaitytuvą,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) kad gautų "Access" taikomųjų programų, kurias naudoja svetainės, aprašą.</span><span class="sxs-lookup"><span data-stu-id="aa96f-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="aa96f-110">Yra keli būdai, kaip perkelti "Access" žiniatinklio duomenų bazių duomenis:</span><span class="sxs-lookup"><span data-stu-id="aa96f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="aa96f-111">Importuojama į vietinę Access duomenų bazę (. ACCDB) arba "Excel" failą.</span><span class="sxs-lookup"><span data-stu-id="aa96f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="aa96f-112">Taip pat rekomenduojame tyrinėti "Microsoft PowerApps" kaip alternatyvią platformą, kad sukurtumėte žiniatinklio ir mobiliųjų įrenginių verslo sprendimus be kodo.</span><span class="sxs-lookup"><span data-stu-id="aa96f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>