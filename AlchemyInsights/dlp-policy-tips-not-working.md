---
title: DLP strategijos patarimai neveikia
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932594"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="dab3f-102">DLP strategijos patarimo problemos</span><span class="sxs-lookup"><span data-stu-id="dab3f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="dab3f-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="dab3f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dab3f-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="dab3f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dab3f-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="dab3f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dab3f-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="dab3f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dab3f-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="dab3f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dab3f-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="dab3f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dab3f-109">**DLP politikos patarimai**</span><span class="sxs-lookup"><span data-stu-id="dab3f-109">**DLP policy tips**</span></span>

<span data-ttu-id="dab3f-110">Naudojant **DLP strategijas**, vartotojams gali būti pranešta apie strategijos pažeidimą su **strategijos patarimais**.</span><span class="sxs-lookup"><span data-stu-id="dab3f-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="dab3f-111">Administratoriai gali konfigūruoti strategijos patarimus, kurie bus rodomi bandant jų DLP strategiją arba kai strategija veikia visu vykdymo režimu.</span><span class="sxs-lookup"><span data-stu-id="dab3f-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="dab3f-112">Norėdami konfigūruoti strategijos patarimus dėl savo DLP strategijos saugos ir atitikties centre visą vykdymo režimu, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="dab3f-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="dab3f-113">Įsitikinkite, kad DLP **taisyklėje** įgalinti strategijos patarimai, atlikdami [čia](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)nurodytus veiksmus .</span><span class="sxs-lookup"><span data-stu-id="dab3f-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="dab3f-114">Įsitikinkite, kad **jūsų turinys atitinka** tai, ko **reikia** norint suaktyvinti šiame straipsnyje aprašytą taisyklę [čia](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="dab3f-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="dab3f-115">Strategijos patarimai rodomi OWA ir "Outlook".</span><span class="sxs-lookup"><span data-stu-id="dab3f-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="dab3f-116">Tačiau naudojant **"Outlook" 2013 m. arba naujesnę versiją,** strategijos patarimai rodomi tik tam tikromis sąlygomis.</span><span class="sxs-lookup"><span data-stu-id="dab3f-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="dab3f-117">Šios sąlygos išvardytos čia: [Palaikomos "Outlook 2013" arba naujesnės versijos strategijos patarimų rodymo sąlygos](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="dab3f-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="dab3f-118">Jei norite gauti papildomos informacijos apie DLP strategijos patarimų, žr.: [Rodyti strategijos patarimų DLP strategijos](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="dab3f-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  