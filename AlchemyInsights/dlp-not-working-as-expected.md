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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977446"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="049b9-102">DLP neveikia taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="049b9-102">DLP not working as expected</span></span>

<span data-ttu-id="049b9-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="049b9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="049b9-104">**DLP nustatymas**</span><span class="sxs-lookup"><span data-stu-id="049b9-104">**Setting up DLP**</span></span>

<span data-ttu-id="049b9-105">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** "Office 365" neveikia kaip tikėtasi?</span><span class="sxs-lookup"><span data-stu-id="049b9-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="049b9-106">Jei taip, įsitikinkite, kad jūsų **DLP strategija** nustatyta teisingai ir kad jūsų duomenyse yra tai, ko ieškote **DLP politikoje,** kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="049b9-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="049b9-107">DLP strategijos leidžia identifikuoti ir apsaugoti slaptą informaciją jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="049b9-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="049b9-108">Norėdami nustatyti DLP strategijas, naudokite [čia](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)pateikiamą informaciją .</span><span class="sxs-lookup"><span data-stu-id="049b9-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="049b9-109">**Kokių DLP politikos sričių ieškote**</span><span class="sxs-lookup"><span data-stu-id="049b9-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="049b9-110">Naudojant **įtaisytuosius slaptos informacijos tipus** "Office 365" saugos ir atitikties centre, DLP strategijos eis dami šiuos slaptus tipus ieško konkrečių modelių ir elementų.</span><span class="sxs-lookup"><span data-stu-id="049b9-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="049b9-111">**Įtaisytieji slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="049b9-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="049b9-112">Informacijos apie įtaisytuosius slaptus tipus ir tai, ko ieško DLP strategija, kai aptinkamas slaptus tipus, žr.: [Ko ieško slaptos informacijos tipai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="049b9-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="049b9-113">**Pasirinktiniai slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="049b9-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="049b9-114">Jei bandote kurti pasirinktinius slaptos informacijos tipus, naudokite šį straipsnį, kad sužinotumėte, kaip sukurti pasirinktinį slaptą tipą: [Pasirinktinio slaptos informacijos tipo kūrimas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="049b9-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="049b9-115">**DLP strategijos tikrinimas**</span><span class="sxs-lookup"><span data-stu-id="049b9-115">**Test a DLP policy**</span></span>

<span data-ttu-id="049b9-116">Norėdami patikrinti duomenis naudodami įtaisytąjį arba tinkintą slaptos informacijos tipą, naudokite parinktį **Bandymo tipas** dalyje **Slaptus slaptus informacijos** > **tipus**klasifikavimas .</span><span class="sxs-lookup"><span data-stu-id="049b9-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="049b9-117">Daugiau informacijos [ieškokite Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="049b9-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="049b9-118">**Ataskaitos**</span><span class="sxs-lookup"><span data-stu-id="049b9-118">**Reports**</span></span>
  
- <span data-ttu-id="049b9-119">Gaukite slaptis duomenų įžvalgas naudodami [DLP ataskaitas.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="049b9-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="049b9-120">Peržiūrėkite konkrečią įvykio informaciją su [incidento ataskaita](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="049b9-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
