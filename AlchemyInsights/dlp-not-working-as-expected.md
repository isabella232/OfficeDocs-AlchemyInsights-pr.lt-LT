---
title: DLP neveikia taip, kaip tikėtasi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704421"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="fe831-102">DLP neveikia taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="fe831-102">DLP not working as expected</span></span>

<span data-ttu-id="fe831-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fe831-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="fe831-104">**DLP nustatymas**</span><span class="sxs-lookup"><span data-stu-id="fe831-104">**Setting up DLP**</span></span>

<span data-ttu-id="fe831-105">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** "Office 365" neveikia kaip tikėtasi?</span><span class="sxs-lookup"><span data-stu-id="fe831-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="fe831-106">Jei taip, įsitikinkite, kad jūsų **DLP strategija** nustatyta teisingai ir kad jūsų duomenyse yra tai, ko ieškote **DLP politikoje,** kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="fe831-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="fe831-107">DLP strategijos leidžia identifikuoti ir apsaugoti slaptą informaciją jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="fe831-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="fe831-108">Norėdami nustatyti DLP strategijas, naudokite [čia](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)pateikiamą informaciją .</span><span class="sxs-lookup"><span data-stu-id="fe831-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="fe831-109">**Kokių DLP politikos sričių ieškote**</span><span class="sxs-lookup"><span data-stu-id="fe831-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="fe831-110">Naudojant **įtaisytuosius slaptos informacijos tipus** saugos ir atitikties centruose, DLP strategijos eisdami šiuos slaptus tipus ieško konkrečių modelių ir elementų.</span><span class="sxs-lookup"><span data-stu-id="fe831-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="fe831-111">**Įtaisytieji slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="fe831-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="fe831-112">Informacijos apie įtaisytuosius slaptus tipus ir tai, ko ieško DLP strategija, kai aptinkamas slaptus tipus, žr.: [Ko ieško slaptos informacijos tipai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="fe831-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="fe831-113">**Pasirinktiniai slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="fe831-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="fe831-114">Jei bandote kurti pasirinktinius slaptos informacijos tipus, naudokite šį straipsnį, kad sužinotumėte, kaip sukurti pasirinktinį slaptą tipą: [Pasirinktinio slaptos informacijos tipo kūrimas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="fe831-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="fe831-115">**DLP strategijos tikrinimas**</span><span class="sxs-lookup"><span data-stu-id="fe831-115">**Test a DLP policy**</span></span>

<span data-ttu-id="fe831-116">Norėdami patikrinti duomenis naudodami įtaisytąjį arba tinkintą slaptos informacijos tipą, naudokite parinktį **Bandymo tipas** dalyje **Slaptus slaptus informacijos** > **tipus**klasifikavimas .</span><span class="sxs-lookup"><span data-stu-id="fe831-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="fe831-117">Daugiau informacijos [ieškokite Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="fe831-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="fe831-118">**Ataskaitos**</span><span class="sxs-lookup"><span data-stu-id="fe831-118">**Reports**</span></span>
  
- <span data-ttu-id="fe831-119">Gaukite slaptis duomenų įžvalgas naudodami [DLP ataskaitas.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="fe831-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="fe831-120">Peržiūrėkite konkrečią įvykio informaciją su [incidento ataskaita](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="fe831-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
