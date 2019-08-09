---
title: Darbo eigos paštu nesiunčiamas
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270680"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="1428b-102">Darbo eigos paštu nesiunčiamas</span><span class="sxs-lookup"><span data-stu-id="1428b-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="1428b-103">El. paštas darbo eigos siunčiami visiems vartotojams arba tik tam tikriems vartotojams, arba matote klaidos **el. laiško negalima išsiųsti. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.</span><span class="sxs-lookup"><span data-stu-id="1428b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="1428b-104">Patikrinti, ar vartotojas yra **Visų žmonių** teises grupės (vartotojo informacijos sąraše) šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="1428b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="1428b-105">Paragauti tiesiogiai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1428b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="1428b-106">Jei vartotojas nėra, įsitikinkite, kad vartotojas yra prisijungę prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="1428b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="1428b-107">Jeigu išorinis vartotojas, įsitikinkite, kad jų kvietimą buvo priimtas.</span><span class="sxs-lookup"><span data-stu-id="1428b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="1428b-108">Jei vartotojas teisės grupė, įsitikinkite, ar teisingas el. pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="1428b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="1428b-109">Jei vartotojai el. pašto adresas nėra nustatytas čia, tada sukurti iš mėginio signalą, kad vartotojas, kuris verčia šio vartotojo abonemento sinchronizavimo SharePoint vartotojo profiliai prie šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="1428b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="1428b-110">El. paštas darbo eigos siunčiami svetainių rinkinio administratoriai, bet ne kitiems vartotojams ir pamatyti klaidos \*\*HTTP draudžiama į <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="1428b-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="1428b-111">Žiūrėkite [Prieiga uždrausta kai išsiųstą el. laišką dalyvauja](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="1428b-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="1428b-112">Be to, įsitikinkite, kad **riboto naudojimo vartotojas leidimo lockdown režimas** svetainių rinkinio funkcija neaktyvi.</span><span class="sxs-lookup"><span data-stu-id="1428b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="1428b-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="1428b-113">Related topics</span></span>
<span data-ttu-id="1428b-114">Norite išbandyti Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="1428b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="1428b-115">Sukurti srauto</span><span class="sxs-lookup"><span data-stu-id="1428b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1428b-116">SharePoint ir srauto</span><span class="sxs-lookup"><span data-stu-id="1428b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


