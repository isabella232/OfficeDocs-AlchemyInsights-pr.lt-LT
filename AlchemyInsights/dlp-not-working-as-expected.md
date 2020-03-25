---
title: DLP neveikia taip, kaip tikėtasi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932630"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="52319-102">DLP neveikia taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="52319-102">DLP not working as expected</span></span>

<span data-ttu-id="52319-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="52319-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="52319-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="52319-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="52319-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="52319-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="52319-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="52319-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="52319-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="52319-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="52319-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="52319-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="52319-109">**DLP nustatymas**</span><span class="sxs-lookup"><span data-stu-id="52319-109">**Setting up DLP**</span></span>

<span data-ttu-id="52319-110">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** "Office 365" neveikia kaip tikėtasi?</span><span class="sxs-lookup"><span data-stu-id="52319-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="52319-111">Jei taip, įsitikinkite, kad jūsų **DLP strategija** nustatyta teisingai ir kad jūsų duomenyse yra tai, ko ieškote **DLP politikoje,** kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="52319-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="52319-112">DLP strategijos leidžia identifikuoti ir apsaugoti slaptą informaciją jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="52319-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="52319-113">Norėdami nustatyti DLP strategijas, naudokite [čia](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)pateikiamą informaciją .</span><span class="sxs-lookup"><span data-stu-id="52319-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="52319-114">**Kokių DLP politikos sričių ieškote**</span><span class="sxs-lookup"><span data-stu-id="52319-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="52319-115">Naudojant **įtaisytuosius slaptos informacijos tipus** "Office 365" saugos ir atitikties centre, DLP strategijos eis dami šiuos slaptus tipus ieško konkrečių modelių ir elementų.</span><span class="sxs-lookup"><span data-stu-id="52319-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="52319-116">**Įtaisytieji slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="52319-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="52319-117">Informacijos apie įtaisytuosius slaptus tipus ir tai, ko ieško DLP strategija, kai aptinkamas slaptus tipus, žr.: [Ko ieško slaptos informacijos tipai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="52319-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="52319-118">**Pasirinktiniai slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="52319-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="52319-119">Jei bandote kurti pasirinktinius slaptos informacijos tipus, naudokite šį straipsnį, kad sužinotumėte, kaip sukurti pasirinktinį slaptą tipą: [Pasirinktinio slaptos informacijos tipo kūrimas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="52319-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="52319-120">**DLP strategijos tikrinimas**</span><span class="sxs-lookup"><span data-stu-id="52319-120">**Test a DLP policy**</span></span>

<span data-ttu-id="52319-121">Norėdami patikrinti duomenis naudodami įtaisytąjį arba tinkintą slaptos informacijos tipą, naudokite parinktį **Bandymo tipas** dalyje **Slaptus slaptus informacijos** > **tipus**klasifikavimas .</span><span class="sxs-lookup"><span data-stu-id="52319-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="52319-122">Daugiau informacijos [ieškokite Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="52319-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="52319-123">**Ataskaitos**</span><span class="sxs-lookup"><span data-stu-id="52319-123">**Reports**</span></span>
  
- <span data-ttu-id="52319-124">Gaukite slaptis duomenų įžvalgas naudodami [DLP ataskaitas.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="52319-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="52319-125">Peržiūrėkite konkrečią įvykio informaciją su [incidento ataskaita](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="52319-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
