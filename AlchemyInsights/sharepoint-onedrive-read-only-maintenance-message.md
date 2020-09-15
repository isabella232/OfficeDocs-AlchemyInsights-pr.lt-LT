---
title: Tik skaitomas priežiūros pranešimas, bandant naudoti "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670840"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="fd6d4-102">Tik skaitomas priežiūros pranešimas, bandant naudoti "SharePoint" arba "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="fd6d4-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="fd6d4-103">Kai bandoma naudoti "SharePoint" arba "OneDrive", kad būtų galima atlikti vieną iš šių scenarijų, vartotojams gali būti **skirtas tik skaityti skirtas priežiūros** pranešimas.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="fd6d4-104">Suplanuota arba aktyvi priežiūros veikla.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="fd6d4-105">Patikrinkite, ar jie naršyti [pranešimų centre](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="fd6d4-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="fd6d4-106">Didelis prioritetas, aktyvus tarnybos incidentas, kuris gali įvykti.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="fd6d4-107">Patikrinkite, ar yra kokių nors klausimų, susijusių su [tarnybų sveikata](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="fd6d4-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="fd6d4-108">Nedidelį automatinį gijimo atkūrimo scenarijų, kuris gali vykti dėl netikėtų įvykių serveriuose, kurie gali trukti trumpiau nei 30 min.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="fd6d4-109">Nėra pranešimų centro arba tarnybos sveikatos postų dėl šių nedidelių atgrąžintų sumų, bet jums turėtų vėl būti taikomas įprastas labai greitai.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="fd6d4-110">Labai retais atvejais stebėjome, kad vienas iš trijų anksčiau nurodytų scenarijų buvo priežastis, o tarnyba atkurta, tačiau vartotojų naršyklės talpykla nebuvo pašalinta.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="fd6d4-111">Prieš naršydami svetainėje pabandykite išvalyti naršyklės talpyklą.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="fd6d4-112">Naršyklėje "Microsoft Edge" pasirinkite **Parametrai**, tada pasirinkite **Privatumas ir sauga**.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="fd6d4-113">Dalyje **valyti naršymą**pasirinkite **pasirinkti, ką išvalyti**.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="fd6d4-114">Pasirinkite **slapukai ir įrašyti svetainės duomenys**, tada pasirinkite **valyti**.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="fd6d4-115">Šie veiksmai gali skirtis, kai naudojamos kitos naršyklės, pvz., "Mozilla Firefox" arba "Google Chrome".</span><span class="sxs-lookup"><span data-stu-id="fd6d4-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="fd6d4-116">Kita galimybė – atidaryti "SharePoint" svetainę arba "OneDrive" naujame "InPrivate" lange.</span><span class="sxs-lookup"><span data-stu-id="fd6d4-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>