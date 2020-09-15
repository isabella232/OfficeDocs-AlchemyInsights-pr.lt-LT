---
title: "\"Access\" tarnybos išėjimas į pensiją"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698690"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3426e-102">"Access" tarnybos išėjimas į pensiją</span><span class="sxs-lookup"><span data-stu-id="3426e-102">Access services retirement</span></span>

<span data-ttu-id="3426e-103">Kaip iš pradžių paskelbėme "MC97576", kovo 2017, ir toliau bendraudavo per praėjusius metus "Access" tarnybos yra išėjusiems.</span><span class="sxs-lookup"><span data-stu-id="3426e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="3426e-104">Kitas šio proceso etapas bus "Access" žiniatinklio duomenų bazių, kurios naudoja "SharePoint" sąrašus kaip pagrindinę duomenų saugyklą, pašalinimas.</span><span class="sxs-lookup"><span data-stu-id="3426e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3426e-105">**Kaip tai veikia?**</span><span class="sxs-lookup"><span data-stu-id="3426e-105">**How does this affect me?**</span></span>

<span data-ttu-id="3426e-106">Nuo birželio "2019", mes sustabdysime naujų "Access" duomenų bazių kūrimą "SharePoint Online" ir išjungsime paslaugą ir likusias taikomąsias programas iki balandžio 2020.</span><span class="sxs-lookup"><span data-stu-id="3426e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3426e-107">**Ką reikia daryti norint pasirengti šiam pakeitimui?**</span><span class="sxs-lookup"><span data-stu-id="3426e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3426e-108">Raginame sukurti savo organizacijos "Access" žiniatinklio duomenų bazių perėjimo planą.</span><span class="sxs-lookup"><span data-stu-id="3426e-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="3426e-109">Administratoriai gali naudoti " [SharePoint Access" taikomosios programos skaitytuvą](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , kad gautų "Access" taikomųjų programų, kurias naudoja svetainės, aprašą.</span><span class="sxs-lookup"><span data-stu-id="3426e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="3426e-110">Yra keli būdai, kaip perkelti "Access" žiniatinklio duomenų bazių duomenis:</span><span class="sxs-lookup"><span data-stu-id="3426e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3426e-111">Importavimas į vietinę "Access" duomenų bazę (. ACCDB) arba "Excel" faile.</span><span class="sxs-lookup"><span data-stu-id="3426e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3426e-112">Taip pat rekomenduojame ieškoti "Microsoft PowerApps" kaip alternatyvi platforma, kad sukurtumėte verslo sprendimus žiniatinklyje ir mobiliuosiuose įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="3426e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>