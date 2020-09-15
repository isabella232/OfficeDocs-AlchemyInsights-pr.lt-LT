---
title: Turinys nerodomas "SharePoint" ieškos rezultatuose
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713138"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="ec6d8-102">Turinys nerodomas "SharePoint" ieškos rezultatuose</span><span class="sxs-lookup"><span data-stu-id="ec6d8-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="ec6d8-103">Vadovaukitės šiais trikčių diagnostikos veiksmais, kai numatomas turinys nerodomas ieškos rezultatuose:</span><span class="sxs-lookup"><span data-stu-id="ec6d8-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="ec6d8-104">Patikrinkite, ar **svetainė** , kurioje yra numatomas turinys, yra nustatyta leisti turiniui Rodyti ieškos rezultatuose.</span><span class="sxs-lookup"><span data-stu-id="ec6d8-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ec6d8-105">Atlikite veiksmus, aprašytus skyriuje [svetainės turinio rodymas ieškos rezultatuose](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="ec6d8-106">Patikrinkite, ar **sąraše** ar **bibliotekoje** , kurioje yra numatomas turinys, nustatyta leisti turiniui Rodyti ieškos rezultatuose.</span><span class="sxs-lookup"><span data-stu-id="ec6d8-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ec6d8-107">Atlikite veiksmus, aprašytus skyriuje [turinio rodymas sąrašuose arba bibliotekose ieškos rezultatuose](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="ec6d8-108">Patikrinkite, ar puslapio, dokumento arba pasirinktinio puslapio maketas publikuojamas kaip **pagrindinė versija.**</span><span class="sxs-lookup"><span data-stu-id="ec6d8-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="ec6d8-109">Atlikdami 3 veiksmą [ieška nepateikia visų "SharePoint Online" rezultatų](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="ec6d8-110">Patikrinkite, ar vartotojas turi **teisę** peržiūrėti turinį.</span><span class="sxs-lookup"><span data-stu-id="ec6d8-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="ec6d8-111">Atlikite veiksmus, pateiktus " [SharePoint" teisių lygių supratimas](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="ec6d8-112">Jei ieškos schema buvo pakeista įtraukiant naują valdomą ypatybę, redaguojant valdomą ypatybę arba pašalinus valdomą ypatybę, reikia atlikti aptikimą ir perindeksuoti užklausą.</span><span class="sxs-lookup"><span data-stu-id="ec6d8-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="ec6d8-113">Iš **naujo rodykite** turinį atlikdami veiksmus, pateiktus [rankiniu būdu, kad būtų nuskaitant ir iš naujo indeksuojamos svetainės, bibliotekos arba sąrašo](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="ec6d8-114">Tai gali šiek tiek užtrukti, palaukite 24 valandas prieš patikrindami rezultatus dar kartą.</span><span class="sxs-lookup"><span data-stu-id="ec6d8-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="ec6d8-115">Daugiau informacijos ieškokite [turinio įgalinimas svetainėje, kad būtų galima ieškoti](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="ec6d8-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
