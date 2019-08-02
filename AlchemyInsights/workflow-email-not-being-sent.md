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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059611"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="d4cef-102">Darbo eigos paštu nesiunčiamas</span><span class="sxs-lookup"><span data-stu-id="d4cef-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="d4cef-103">El. paštas darbo eigos siunčiami visiems vartotojams arba tik tam tikriems vartotojams, arba matote klaidos **el. laiško negalima išsiųsti. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.</span><span class="sxs-lookup"><span data-stu-id="d4cef-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="d4cef-104">Patikrinti, ar vartotojas yra **Visų žmonių** teises grupės (vartotojo informacijos sąraše) šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="d4cef-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="d4cef-105">Paragauti tiesiogiai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="d4cef-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="d4cef-106">Jei vartotojas nėra, įsitikinkite, kad vartotojas yra prisijungę prie puslapio.</span><span class="sxs-lookup"><span data-stu-id="d4cef-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="d4cef-107">Jeigu išorinis vartotojas, įsitikinkite, kad jų kvietimą buvo priimtas.</span><span class="sxs-lookup"><span data-stu-id="d4cef-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="d4cef-108">Jei vartotojas teisės grupė, įsitikinkite, ar teisingas el. pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="d4cef-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="d4cef-109">Jei vartotojai el. pašto adresas nėra nustatytas čia, tada sukurti iš mėginio signalą, kad vartotojas, kuris verčia šio vartotojo abonemento sinchronizavimo SharePoint vartotojo profiliai prie šio svetainių rinkinio.</span><span class="sxs-lookup"><span data-stu-id="d4cef-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="d4cef-110">El. paštas darbo eigos siunčiami svetainių rinkinio administratoriai, bet ne kitiems vartotojams ir pamatyti klaidos \*\*HTTP draudžiama į <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="d4cef-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="d4cef-111">Žiūrėkite [Prieiga uždrausta kai išsiųstą el. laišką dalyvauja](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="d4cef-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="d4cef-112">Be to, įsitikinkite, kad **riboto naudojimo vartotojas leidimo lockdown režimas** svetainių rinkinio funkcija neaktyvi.</span><span class="sxs-lookup"><span data-stu-id="d4cef-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="d4cef-113">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="d4cef-113">Related topics</span></span>
- [<span data-ttu-id="d4cef-114">Sukurti srauto</span><span class="sxs-lookup"><span data-stu-id="d4cef-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d4cef-115">SharePoint ir srauto</span><span class="sxs-lookup"><span data-stu-id="d4cef-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


