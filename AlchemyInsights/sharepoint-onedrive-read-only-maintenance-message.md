---
title: Tik skaitomas techninės priežiūros pranešimas bandant naudoti SharePoint arba "OneDrive"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051289"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="57d18-102">Tik skaitomas techninės priežiūros pranešimas bandant naudoti SharePoint arba "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="57d18-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="57d18-103">Vartotojai gali gauti **tik skaitomas priežiūros** pranešimas bandant naudoti SharePoint arba OneDrive vieną iš šių scenarijų.</span><span class="sxs-lookup"><span data-stu-id="57d18-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="57d18-104">Suplanuota arba aktyvi priežiūros veikla.</span><span class="sxs-lookup"><span data-stu-id="57d18-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="57d18-105">Patikrinkite, ar jie pereidami į [pranešimų centrą](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="57d18-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="57d18-106">Aukšto prioriteto, aktyvus tarnybos incidentas, kuris gali būti vyksta.</span><span class="sxs-lookup"><span data-stu-id="57d18-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="57d18-107">Jei norite sužinoti apie visus patarimus ar incidentus, žiūrėkite į [paslaugos sveikatą](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="57d18-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="57d18-108">Nepilnametis Auto-gijimo atkūrimo scenarijus, kad galėtų būti vyksta dėl netikėtų įvykių serveriuose, kurie gali trukti mažiau nei 30 min.</span><span class="sxs-lookup"><span data-stu-id="57d18-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="57d18-109">Nėra pranešimų centras arba tarnybos sveikatos pranešimų šių nedidelių susigrąžinti, bet jums turėtų būti grįžti prie normalaus labai greitai.</span><span class="sxs-lookup"><span data-stu-id="57d18-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="57d18-110">Labai retais atvejais mes nustatėme, kad vienas iš trijų pirmiau išvardytų scenarijų buvo priežastis, ir paslauga buvo atkurta, bet vartotojų naršyklė talpyklos nebuvo išvalytas iki.</span><span class="sxs-lookup"><span data-stu-id="57d18-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="57d18-111">Prieš eidami į svetainę, bandykite išvalyti naršyklės talpyklą.</span><span class="sxs-lookup"><span data-stu-id="57d18-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="57d18-112">Naršyklėje "Microsoft Edge" pasirinkite **Parametrai**, tada pasirinkite **Privatumas ir sauga**.</span><span class="sxs-lookup"><span data-stu-id="57d18-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="57d18-113">Dalyje **išvalyti naršymą**pasirinkite **pasirinkti, ką išvalyti**.</span><span class="sxs-lookup"><span data-stu-id="57d18-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="57d18-114">Pasirinkite **slapukai ir išsaugoti svetainės duomenys**, ir pasirinkite **išvalyti**.</span><span class="sxs-lookup"><span data-stu-id="57d18-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="57d18-115">Šie veiksmai gali skirtis naudojant kitas naršykles, pvz., "Mozilla Firefox" arba "Google Chrome".</span><span class="sxs-lookup"><span data-stu-id="57d18-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="57d18-116">Kita galimybė būtų atidaryti SharePoint svetainę arba "OneDrive" naujame "InPrivate" lange.</span><span class="sxs-lookup"><span data-stu-id="57d18-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>