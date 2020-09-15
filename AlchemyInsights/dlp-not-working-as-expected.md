---
title: DLP veikia ne taip, kaip tikėtasi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679701"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="cd679-102">DLP veikia ne taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="cd679-102">DLP not working as expected</span></span>

<span data-ttu-id="cd679-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="cd679-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="cd679-104">**DLP nustatymas**</span><span class="sxs-lookup"><span data-stu-id="cd679-104">**Setting up DLP**</span></span>

<span data-ttu-id="cd679-105">Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** "Office 365" neveikia?</span><span class="sxs-lookup"><span data-stu-id="cd679-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="cd679-106">Jei taip, įsitikinkite, kad jūsų **DLP strategija** nustatyta tinkamai ir ar jūsų duomenyse yra " **DLP" strategija** , kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="cd679-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="cd679-107">DLP strategijos leidžia nustatyti ir apsaugoti slaptą informaciją jūsų organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="cd679-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="cd679-108">Norėdami sukonfigūruoti DLP strategijas, naudokite [čia](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)esančią informaciją.</span><span class="sxs-lookup"><span data-stu-id="cd679-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="cd679-109">**Ko ieško DLP strategijos**</span><span class="sxs-lookup"><span data-stu-id="cd679-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="cd679-110">Naudojant **įtaisytuosius delikačios informacijos tipus** saugos ir atitikties centruose, DLP strategijos ieško konkrečių modelių ir elementų aptikus šiuos jautrius tipus.</span><span class="sxs-lookup"><span data-stu-id="cd679-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="cd679-111">**Įtaisytieji slapto pobūdžio informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="cd679-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="cd679-112">Informacijos apie įtaisytuosius jautrius tipus ir tai, ką nustato DLP strategija, kai aptinkami slapti tipai, žiūrėkite: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="cd679-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="cd679-113">**Pasirinktinio slapto pobūdžio informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="cd679-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="cd679-114">Jei bandote sukurti pasirinktinio slapto pobūdžio informacijos tipus, informacijos apie tai, kaip sukurti pasirinktinę slaptą tipą, naudokite toliau pateiktą straipsnį: [pasirinktinio slapto informacijos tipo kūrimas](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="cd679-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="cd679-115">**DLP strategijos tikrinimas**</span><span class="sxs-lookup"><span data-stu-id="cd679-115">**Test a DLP policy**</span></span>

<span data-ttu-id="cd679-116">Norėdami patikrinti savo duomenis įtaisytuoju arba pasirinktiniu slaptos informacijos tipu, naudokite parinktį **tikrinimo tipas** , esančią dalyje **klasifikacijos**  >  **slaptos informacijos tipai**.</span><span class="sxs-lookup"><span data-stu-id="cd679-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="cd679-117">Daugiau informacijos ieškokite [pasirinktinio slapto informacijos tipų tikrinimas](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="cd679-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="cd679-118">**Ataskaitas**</span><span class="sxs-lookup"><span data-stu-id="cd679-118">**Reports**</span></span>
  
- <span data-ttu-id="cd679-119">Gaukite slaptų duomenų įžvalgų naudodami [DLP ataskaitas.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="cd679-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="cd679-120">Konkrečios įvykio informacijos peržiūra su [incidento ataskaita](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="cd679-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
