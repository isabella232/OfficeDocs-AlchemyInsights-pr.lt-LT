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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530889"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="ff9fa-102">Darbo eigos paštu nesiunčiamas SharePoint sąrašo arba bibliotekos</span><span class="sxs-lookup"><span data-stu-id="ff9fa-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="ff9fa-103">El. paštas darbo eigos siunčiami visiems vartotojams arba tik tam tikriems vartotojams, arba matote klaidos **el. laiško negalima išsiųsti. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="ff9fa-104">Patikrinti, ar vartotojas yra **Visų žmonių** teises grupės (vartotojo informacijos sąraše) šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ff9fa-105">Paragauti tiesiogiai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ff9fa-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="ff9fa-106">Jei vartotojas nėra, įsitikinkite, kad vartotojas yra prisijungę prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="ff9fa-107">Jeigu išorinis vartotojas, įsitikinkite, kad jų kvietimą buvo priimtas.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="ff9fa-108">Jei vartotojas teisės grupė, įsitikinkite, ar teisingas el. pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="ff9fa-109">Jei vartotojai el. pašto adresas nėra nustatytas čia, tada sukurti iš mėginio signalą, kad vartotojas, kuris verčia šio vartotojo abonemento sinchronizavimo SharePoint vartotojo profiliai prie šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ff9fa-110">El. paštas darbo eigos siunčiami svetainių rinkinio administratoriai, bet ne kitiems vartotojams ir pamatyti klaidos **HTTP draudžiama į <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="ff9fa-111">Pamatyti [Access Denied siunčiant el. laišką SharePoint grupei](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="ff9fa-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="ff9fa-112">Be to, įsitikinkite, kad **riboto naudojimo vartotojas leidimo lockdown režimas** svetainių rinkinio funkcija neaktyvi.</span><span class="sxs-lookup"><span data-stu-id="ff9fa-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="ff9fa-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="ff9fa-113">Related topics</span></span>
<span data-ttu-id="ff9fa-114">Norite išbandyti Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ff9fa-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ff9fa-115">Sukurti srauto</span><span class="sxs-lookup"><span data-stu-id="ff9fa-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ff9fa-116">SharePoint ir srauto</span><span class="sxs-lookup"><span data-stu-id="ff9fa-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


