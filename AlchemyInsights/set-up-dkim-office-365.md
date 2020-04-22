---
title: Nustatyti DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645680"
---
# <a name="setup-dkim"></a><span data-ttu-id="2d5f8-102">Nustatyti DKIM</span><span class="sxs-lookup"><span data-stu-id="2d5f8-102">Setup DKIM</span></span>

<span data-ttu-id="2d5f8-103">Išsami instrukcija konfigūruoti DKIM pasirinktinių domenų Microsoft 365 yra [čia](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2d5f8-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="2d5f8-104">**Kiekvienam** pasirinktiniam domenui turite sukurti **du** DKIM CNAME įrašus domeno DNS išteklių nuomos tarnyboje (paprastai domenų registratoriuje).</span><span class="sxs-lookup"><span data-stu-id="2d5f8-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="2d5f8-105">Pavyzdžiui, contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įrašų: du contoso.com ir du fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="2d5f8-106">DKIM CNAME įrašai **kiekvienam** pasirinktiniam domenui naudoja šiuos formatus:</span><span class="sxs-lookup"><span data-stu-id="2d5f8-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="2d5f8-107">**Pagrindinio kompiuterio vardas**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2d5f8-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2d5f8-108">**Nukreipia adresu arba reikšmė:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2d5f8-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2d5f8-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2d5f8-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="2d5f8-110">**Pagrindinio kompiuterio vardas**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="2d5f8-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="2d5f8-111">**Nukreipia adresu arba reikšmė:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="2d5f8-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="2d5f8-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="2d5f8-112">**TTL**: 3600</span></span>

   <span data-ttu-id="2d5f8-113">\<DomainGUID\> yra pasirinktinio domeno `.mail.protection.outlook.com` tinkinto MX įrašo tekstas į kairę (pvz., `contoso-com` domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2d5f8-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="2d5f8-114">\<InitialDomain\> yra domenas, kurį naudojote prisiregistruodami naudoti "Microsoft 365" (pvz., contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="2d5f8-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="2d5f8-115">Sukūrę pasirinktinių domenų CNAME įrašus, atlikite toliau nurodytas instrukcijas:</span><span class="sxs-lookup"><span data-stu-id="2d5f8-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="2d5f8-116">A.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-116">a.</span></span> <span data-ttu-id="2d5f8-117">[prisijunkite prie "Microsoft 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) naudodami savo darbo arba mokymo įstaigos paskyrą.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="2d5f8-118">B.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-118">b.</span></span> <span data-ttu-id="2d5f8-119">Viršutiniame kairiajame kampe pasirinkite taikomųjų programų vykdyklės piktogramą ir pasirinkite **Administravimas**.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="2d5f8-120">C.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-120">c.</span></span> <span data-ttu-id="2d5f8-121">Apatinėje kairiojoje naršymo srityje išplėskite **Administravimas** ir pasirinkite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="2d5f8-122">D.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-122">d.</span></span> <span data-ttu-id="2d5f8-123">Eikite į **Apsauga** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="2d5f8-124">E.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-124">e.</span></span> <span data-ttu-id="2d5f8-125">Pasirinkite domeną, tada pasirinkite **Įgalinti** **šio domeno pranešimams pasirašyti su DKIM parašais**.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="2d5f8-126">Pakartokite šį veiksmą su kiekvienu pasirinktiniu domenu.</span><span class="sxs-lookup"><span data-stu-id="2d5f8-126">Repeat this step for each custom domain.</span></span>
