---
title: Prieigos paslaugų išėjimo į pensiją
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769453"
---
# <a name="access-services-retirement"></a><span data-ttu-id="4ba6e-102">Prieigos paslaugų išėjimo į pensiją</span><span class="sxs-lookup"><span data-stu-id="4ba6e-102">Access services retirement</span></span>

<span data-ttu-id="4ba6e-103">Kaip mes iš pradžių buvo paskelbta MC97576, – 2017 m. kovo ir toliau bendrauti per pastaruosius metus prieigos paslaugų pareigūn "Office 365".</span><span class="sxs-lookup"><span data-stu-id="4ba6e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="4ba6e-104">Kitame etape šiame procese bus pašalinti prieigos žiniatinklio duomenų bazės, kuriuose SharePoint sąrašai yra jų pagrindinės duomenų saugyklos.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="4ba6e-105">**Kaip tai mane paveiks?**</span><span class="sxs-lookup"><span data-stu-id="4ba6e-105">**How does this affect me?**</span></span>

<span data-ttu-id="4ba6e-106">Nuo 2019 m. birželio, mes nustoti kurti naują Access duomenų bazių SharePoint Online ir uždaryti paslaugos ir visos likusios programos iki 2020 m. balandžio.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="4ba6e-107">**Ką turiu daryti, kad rengiamasi šiam ekonomikos virsmui?**</span><span class="sxs-lookup"><span data-stu-id="4ba6e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="4ba6e-108">Skatiname jus kurti perėjimo planą jūsų organizacijos prieigos žiniatinklio duomenų bazės.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="4ba6e-109">Administratoriai naudoti [SharePoint prieigos programėlė skaitytuvas](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) gauti prieigos programos, kurios svetainių naudoja aprašą.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="4ba6e-110">Yra keli būdai perkelti prieigos interneto duomenų bazių duomenis:</span><span class="sxs-lookup"><span data-stu-id="4ba6e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="4ba6e-111">Importuoti į vietinės prieigos duomenų bazės (. ACCDB) arba "Excel" failą.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="4ba6e-112">Mes taip pat rekomenduojame ieškoti "Microsoft" PowerApps kaip alternatyvi platforma sukurti be kodo verslo valdymo sprendimus, žiniatinklio ir mobiliuosius įrenginius.</span><span class="sxs-lookup"><span data-stu-id="4ba6e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>