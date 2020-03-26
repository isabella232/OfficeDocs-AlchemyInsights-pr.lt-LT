---
title: Nepavyksta prisijungti prie „Teams“ dėl klaidos autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932038"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="38d8f-102">Nepavyksta prisijungti prie „Teams“ dėl klaidos autologon.microsoftazuread-sso taškas com:443</span><span class="sxs-lookup"><span data-stu-id="38d8f-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="38d8f-103">Jei kaip O365 autentifikavimas įjungta sklandi SSO, URL „autologon.microsoftazuread-sso.com“ gali prireikti įtraukti į intraneto svetaines.</span><span class="sxs-lookup"><span data-stu-id="38d8f-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="38d8f-104">Jei ji anksčiau buvo įtraukta į patikimas svetaines ir yra naudojama sklandi SSO, ji turi būti pašalinta iš patikimų svetainių.</span><span class="sxs-lookup"><span data-stu-id="38d8f-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="38d8f-105">Peržiūrėkite [Sklandžios SSO trikčių diagnostikos kontrolinį sąrašą](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="38d8f-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="38d8f-106">Atlikite šiuos veiksmus, kad įtrauktumėte URL į intraneto svetainių sąrašą:</span><span class="sxs-lookup"><span data-stu-id="38d8f-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="38d8f-107">Atidarykite „Internet Explorer“ spustelėdami mygtuką **Pradžia**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="38d8f-108">Ieškos lauke įveskite „Internet Explorer“, tada rezultatų sąraše spustelėkite **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="38d8f-109">Spustelėkite **Įrankiai**, tada spustelėkite **Interneto parinktys**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="38d8f-110">Spustelėkite skirtuką **Sauga**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="38d8f-111">Spustelėkite **Vietinio intraneto svetainės**, tada spustelėkite mygtuką **svetainės** ir mygtuką **Išsamiai**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="38d8f-112">Įveskite svetainės URL ir spustelėkite **Įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="38d8f-113">Baigę spustelėkite **Uždaryti**.</span><span class="sxs-lookup"><span data-stu-id="38d8f-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="38d8f-114">Daugiau informacijos žr. [Sklandžios SSO, skirtos O365, diegimo dokumentacija](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (apima strategija pagrįstą procesą, kad būtų galima įtraukti URL į intraneto svetaines atliekant 3 veiksmą).</span><span class="sxs-lookup"><span data-stu-id="38d8f-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
