---
title: Prieigos prie išėjimo į pensiją paslaugos
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747792"
---
# <a name="access-services-retirement"></a><span data-ttu-id="af747-102">Prieigos prie išėjimo į pensiją paslaugos</span><span class="sxs-lookup"><span data-stu-id="af747-102">Access services retirement</span></span>

<span data-ttu-id="af747-103">Kaip mes iš pradžių paskelbė MC97576, kovo 2017, ir toliau bendrauti per pastaruosius metus prieigos paslaugos yra pensininkas iš Office 365.</span><span class="sxs-lookup"><span data-stu-id="af747-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="af747-104">Kitas šio proceso etapas bus pašalinti prieigos žiniatinklio duomenų bazių, kurios naudoja SharePoint sąrašus kaip jų pagrindinės duomenų saugyklos.</span><span class="sxs-lookup"><span data-stu-id="af747-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="af747-105">**Kaip tai įtakoja mane?**</span><span class="sxs-lookup"><span data-stu-id="af747-105">**How does this affect me?**</span></span>

<span data-ttu-id="af747-106">Nuo birželio 2019, mes nustosime kurti naujas Access duomenų bazių SharePoint Online ir uždaryti paslaugą ir visas likusias programas iki balandžio 2020.</span><span class="sxs-lookup"><span data-stu-id="af747-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="af747-107">**Ką reikia daryti, kad pasiruoštumėte šiam pasikeittam pokyčiams?**</span><span class="sxs-lookup"><span data-stu-id="af747-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="af747-108">Raginame sukurti jūsų organizacijos "Access" žiniatinklio duomenų bazių perėjimo planą.</span><span class="sxs-lookup"><span data-stu-id="af747-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="af747-109">Administratoriai gali naudoti [SharePoint Access programos skaitytuvą](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) Norėdami gauti "Access" programėlių, kurias naudoja svetainės, aprašą.</span><span class="sxs-lookup"><span data-stu-id="af747-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="af747-110">Yra keli būdai, kaip perkelti prieigą prie žiniatinklio duomenų bazių duomenų:</span><span class="sxs-lookup"><span data-stu-id="af747-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="af747-111">Importuojama į vietinę Access duomenų bazę (. ACCDB) arba "Excel" failui.</span><span class="sxs-lookup"><span data-stu-id="af747-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="af747-112">Taip pat rekomenduojame tyrinėti "Microsoft PowerApps" kaip alternatyvią platformą, kad būtų sukurti be kodo verslo sprendimai žiniatinklio ir mobiliesiems įrenginiams.</span><span class="sxs-lookup"><span data-stu-id="af747-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>