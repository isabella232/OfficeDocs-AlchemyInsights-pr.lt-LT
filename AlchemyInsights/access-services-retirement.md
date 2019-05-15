---
title: Prieigos paslaugų išėjimo į pensiją
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973934"
---
# <a name="access-services-retirement"></a><span data-ttu-id="14abb-102">Prieigos paslaugų išėjimo į pensiją</span><span class="sxs-lookup"><span data-stu-id="14abb-102">Access services retirement</span></span>

<span data-ttu-id="14abb-103">Kaip mes iš pradžių buvo paskelbta MC97576, – 2017 m. kovo ir toliau bendrauti per pastaruosius metus prieigos paslaugų pareigūn "Office 365".</span><span class="sxs-lookup"><span data-stu-id="14abb-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="14abb-104">Kitame etape šiame procese bus pašalinti prieigos žiniatinklio duomenų bazės, kuriuose SharePoint sąrašai yra jų pagrindinės duomenų saugyklos.</span><span class="sxs-lookup"><span data-stu-id="14abb-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="14abb-105">Kaip tai mane paveiks?</span><span class="sxs-lookup"><span data-stu-id="14abb-105">How does this affect me?</span></span>

<span data-ttu-id="14abb-106">Nuo 2019 m. birželio, mes nustoti kurti naują Access duomenų bazių SharePoint Online ir uždaryti paslaugos ir visos likusios programos iki 2020 m. balandžio.</span><span class="sxs-lookup"><span data-stu-id="14abb-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="14abb-107">Ką turiu daryti, kad rengiamasi šiam ekonomikos virsmui?</span><span class="sxs-lookup"><span data-stu-id="14abb-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="14abb-108">Skatiname jus kurti perėjimo planą jūsų organizacijos prieigos žiniatinklio duomenų bazės.</span><span class="sxs-lookup"><span data-stu-id="14abb-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="14abb-109">Administratoriai naudoti [SharePoint prieigos programėlė skaitytuvas](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) gauti prieigos programos, kurios svetainių naudoja aprašą.</span><span class="sxs-lookup"><span data-stu-id="14abb-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="14abb-110">Yra keli būdai perkelti prieigos interneto duomenų bazių duomenis:</span><span class="sxs-lookup"><span data-stu-id="14abb-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="14abb-111">Importuoti į vietinės prieigos duomenų bazės (. ACCDB) arba "Excel" failą.</span><span class="sxs-lookup"><span data-stu-id="14abb-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="14abb-112">Mes taip pat rekomenduojame ieškoti "Microsoft" PowerApps kaip alternatyvi platforma sukurti be kodo verslo valdymo sprendimus, žiniatinklio ir mobiliuosius įrenginius.</span><span class="sxs-lookup"><span data-stu-id="14abb-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>