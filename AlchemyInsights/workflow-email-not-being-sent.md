---
title: Neatsiųstas darbo eigos laiškas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748997"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="7278c-102">"SharePoint" sąrašui arba bibliotekai nesiunčiama darbo eigos el. paštas</span><span class="sxs-lookup"><span data-stu-id="7278c-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="7278c-103">El. laiškai iš darbo eigų nesiunčiami visiems vartotojams arba tik konkretiems vartotojams arba rodoma klaida, **kai el. laiško išsiųsti negalima. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.</span><span class="sxs-lookup"><span data-stu-id="7278c-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="7278c-104">Patikrinkite, ar vartotojas nėra to svetainių rinkinio grupėje **Visos žmonių** teisės (vartotojų informacijos sąrašas).</span><span class="sxs-lookup"><span data-stu-id="7278c-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="7278c-105">Pavyzdinis tiesioginis URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="7278c-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="7278c-106">Jei vartotojo nėra, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="7278c-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="7278c-107">Jei tai išorinis vartotojas, įsitikinkite, kad jų kvietimas priimtas.</span><span class="sxs-lookup"><span data-stu-id="7278c-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="7278c-108">Jei vartotojas yra grupėje teisės, įsitikinkite, kad teisingas elektroninio pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="7278c-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="7278c-109">Jei vartotojas elektroninio pašto adresas nustatytas čia, tada sukurkite įspėjimų apie tą vartotoją, kuris verčia tos vartotojo paskyros sinchronizavimą iš "SharePoint" vartotojų profilių su šiuo svetainių rinkiniu.</span><span class="sxs-lookup"><span data-stu-id="7278c-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="7278c-110">El. laiškai iš darbo eigų siunčiami svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir matyti klaidos **http uždraustas <span>https:</span>//URL/_vti_bin/Client.xvc.sp.utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="7278c-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="7278c-111">[Jei siunčiate laišką "SharePoint" grupei, žiūrėkite prieiga uždrausta](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="7278c-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="7278c-112">Taip pat patikrinkite, ar neaktyvi " **Access" vartotojo teisių blokavimo režimo** svetainių rinkinio funkcija.</span><span class="sxs-lookup"><span data-stu-id="7278c-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="7278c-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="7278c-113">Related topics</span></span>
<span data-ttu-id="7278c-114">Norite išbandyti "Microsoft Flow" "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="7278c-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7278c-115">Kurti srautą</span><span class="sxs-lookup"><span data-stu-id="7278c-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7278c-116">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="7278c-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


