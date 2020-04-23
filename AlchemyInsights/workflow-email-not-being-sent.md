---
title: Darbo eigos el. laiškas nesiunčiamas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766141"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="323a7-102">Darbo eigos el. laiškas nesiunčiamas SharePoint sąrašui arba bibliotekai</span><span class="sxs-lookup"><span data-stu-id="323a7-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="323a7-103">El. laiškai iš darbo eigų siunčiami ne visiems vartotojams arba tik konkretiems vartotojams arba matote **klaidą El. laiško išsiųsti negalima. Įsitikinkite, kad el. laiške yra tinkamas gavėjas**.</span><span class="sxs-lookup"><span data-stu-id="323a7-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="323a7-104">Patikrinkite, ar vartotojas yra to svetainių rinkinio teisių grupėje **Visi žmonės** (vartotojo informacijos sąraše).</span><span class="sxs-lookup"><span data-stu-id="323a7-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="323a7-105">Tiesioginio URL<tenant>pavyzdys: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="323a7-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="323a7-106">Jei vartotojo nėra, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="323a7-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="323a7-107">Jei jis yra išorinis vartotojas, įsitikinkite, kad jų kvietimas buvo priimtas.</span><span class="sxs-lookup"><span data-stu-id="323a7-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="323a7-108">Jei vartotojas yra teisių grupėje, įsitikinkite, kad el. pašto adresas yra teisingas.</span><span class="sxs-lookup"><span data-stu-id="323a7-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="323a7-109">Jei čia vartotojų el. pašto adresas nenustatytas, sukurkite to vartotojo įspėjimo pavyzdį, kuris verčia sinchronizuoti tą vartotojo abonementą iš "SharePoint" vartotojų profilių į šį svetainių rinkinį.</span><span class="sxs-lookup"><span data-stu-id="323a7-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="323a7-110">El. laiškas iš darbo eigų siunčiamas svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir rodoma klaida **HTTP Draudžiama <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="323a7-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="323a7-111">Prieiga [uždrausta, kai siunčiate el. laišką SharePoint grupei](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="323a7-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="323a7-112">Be to, patikrinkite, ar **ribotos prieigos vartotojo teisių užrakinimo režimo** svetainių rinkinio funkcija nėra aktyvi.</span><span class="sxs-lookup"><span data-stu-id="323a7-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="323a7-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="323a7-113">Related topics</span></span>
<span data-ttu-id="323a7-114">Norite išbandyti "Microsoft Flow" "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="323a7-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="323a7-115">Kurti srautą</span><span class="sxs-lookup"><span data-stu-id="323a7-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="323a7-116">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="323a7-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


