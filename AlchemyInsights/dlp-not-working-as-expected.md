---
title: DLP, neveikia kaip tikėtasi
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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941076"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="da216-102">DLP, neveikia kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="da216-102">DLP not working as expected</span></span>

<span data-ttu-id="da216-103">Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** "Office 365" neveikia kaip tikėtasi?</span><span class="sxs-lookup"><span data-stu-id="da216-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="da216-104">Jei taip, įsitikinkite, kad jūsų **DLP strategijos** yra nustatyta teisingai, ir kad jūsų duomenys yra kas **DLP strategijos** ieško kai jis yra vertinamas.</span><span class="sxs-lookup"><span data-stu-id="da216-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="da216-105">**DLP, nustatantį**</span><span class="sxs-lookup"><span data-stu-id="da216-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="da216-106">DLP strategijas leidžia jums nustatyti ir apsaugoti slaptą informaciją savo organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="da216-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="da216-107">Sukonfigūruoti DLP strategijas, naudoti informaciją [čia](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="da216-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="da216-108">**Ieškoti DLP strategijas**</span><span class="sxs-lookup"><span data-stu-id="da216-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="da216-109">Naudojant **įmontuotą slaptos informacijos tipai** Office 365 saugos ir atitikties užtikrinimo centre, DLP strategijas atrodo konkrečiais trafaretais ir elementai, kai aptikti šių jautrių rūšių.</span><span class="sxs-lookup"><span data-stu-id="da216-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="da216-110">**Built-in slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="da216-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="da216-111">Integruotas jautrus tipai ir ką DLP strategijos ieško kai aptikti slaptą tipo informacijos, žr.: [Ieškoti slaptos informacijos tipus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="da216-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="da216-112">**Individualizuotos slaptos informacijos tipai**</span><span class="sxs-lookup"><span data-stu-id="da216-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="da216-113">Jei norite kurti pasirinktinius slaptos informacijos tipus, naudokite šį straipsnį informacijos apie tai, kaip kurti pasirinktinį jautrus tipo: [sukurti pasirinktinį slaptos informacijos tipas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="da216-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="da216-114">**Išbandyti DLP strategijos**</span><span class="sxs-lookup"><span data-stu-id="da216-114">**Test a DLP policy**</span></span>

<span data-ttu-id="da216-115">Norėdami patikrinti savo duomenis su įtaisytus arba pasirinktinius slaptos informacijos tipo, naudokite parinktį **bandymo tipas** pagal **klasifikacijas** > **jautrios informacijos tipai**.</span><span class="sxs-lookup"><span data-stu-id="da216-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="da216-116">Daugiau informacijos ieškokite [bandymo pasirinktinį slaptos informacijos tipus](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="da216-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="da216-117">**Ataskaitos**</span><span class="sxs-lookup"><span data-stu-id="da216-117">**Reports**</span></span>
  
- <span data-ttu-id="da216-118">Gaukite įžvalgų slaptų duomenų su [DLP ataskaitas.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="da216-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="da216-119">Peržiūrėti konkrečią informaciją apie [Incidento](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)atveju.</span><span class="sxs-lookup"><span data-stu-id="da216-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
