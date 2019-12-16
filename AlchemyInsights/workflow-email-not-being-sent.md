---
title: Nesiunčiamas darbo eigos el. laiškas
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049381"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a851a-102">Darbo eigos el. laiškas nesiunčiamas SharePoint sąrašui arba bibliotekai</span><span class="sxs-lookup"><span data-stu-id="a851a-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a851a-103">El. laiškai iš darbo eigų nesiunčiami visiems vartotojams arba tik konkretiems vartotojams, arba matote klaidą **, kurios negalima siųsti el. laišku. Įsitikinkite, kad el. laiške yra galiojantis gavėjas**.</span><span class="sxs-lookup"><span data-stu-id="a851a-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a851a-104">Patikrinkite, ar vartotojas yra **visų asmenų** teisių grupės (vartotojo informacijos sąraše), kad svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="a851a-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a851a-105">Imties tiesioginė URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="a851a-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a851a-106">Jei vartotojas neegzistuoja, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="a851a-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a851a-107">Jei tai išorinis naudotojas, įsitikinkite, kad jo kvietimas buvo priimtas.</span><span class="sxs-lookup"><span data-stu-id="a851a-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a851a-108">Jei teisių grupėje yra vartotojas, įsitikinkite, kad el. pašto adresas teisingas.</span><span class="sxs-lookup"><span data-stu-id="a851a-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a851a-109">Jei vartotojų el. pašto adresas čia nenustatytas, tada sukurkite įspėjimą apie pavyzdį tam vartotojui, kuris priverčia to vartotojo abonemento sinchronizavimą iš "SharePoint" vartotojo profilių į šį svetainių rinkinį.</span><span class="sxs-lookup"><span data-stu-id="a851a-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a851a-110">El. laiškai iš darbo eigų siunčiami svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir rodoma klaida **http uždrausta <span>https:</span>//URL/_vti_bin/Client.xvc.sp.utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="a851a-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a851a-111">Peržiūrėkite [prieiga uždrausta siunčiant el. laišką į SharePoint grupę](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a851a-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a851a-112">Be to, patikrinkite, ar nėra aktyvus **ribotos prieigos vartotojo teisių blokavimo režimu** svetainių rinkinio funkcija.</span><span class="sxs-lookup"><span data-stu-id="a851a-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a851a-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="a851a-113">Related topics</span></span>
<span data-ttu-id="a851a-114">Norite išbandyti "Microsoft Flow" "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="a851a-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a851a-115">Sukurti srautą</span><span class="sxs-lookup"><span data-stu-id="a851a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a851a-116">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="a851a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


