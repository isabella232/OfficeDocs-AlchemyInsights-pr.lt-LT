---
title: "\"DKIM\" sąranka"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808715"
---
# <a name="setup-dkim"></a><span data-ttu-id="ad865-102">"DKIM" sąranka</span><span class="sxs-lookup"><span data-stu-id="ad865-102">Setup DKIM</span></span>

<span data-ttu-id="ad865-103">[Čia](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)rasite instrukcijas, kaip sukonfigūruoti "DKIM" tinkintus domenus programoje "Microsoft 365".</span><span class="sxs-lookup"><span data-stu-id="ad865-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="ad865-104">**Kiekvienam** pasirinktiniam domenui turite sukurti **du** DKIM CNAME įrašus savo domeno DNS išteklių nuomos tarnyboje (paprastai tai yra domenų registratorius).</span><span class="sxs-lookup"><span data-stu-id="ad865-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="ad865-105">Pvz., contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įra ų: du – contoso.com ir du – fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="ad865-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="ad865-106">DKIM CNAME įrašų **kiekvienam** pasirinktiniam domenui naudokite šiuos formatus:</span><span class="sxs-lookup"><span data-stu-id="ad865-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="ad865-107">**Pagrindinio kompiuterio vardas**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ad865-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ad865-108">**Taškai adresu arba reikšmė**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ad865-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ad865-109">" **CTL**": 3600</span><span class="sxs-lookup"><span data-stu-id="ad865-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="ad865-110">**Pagrindinio kompiuterio vardas**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ad865-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ad865-111">**Taškai adresu arba reikšmė**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ad865-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ad865-112">" **CTL**": 3600</span><span class="sxs-lookup"><span data-stu-id="ad865-112">**TTL**: 3600</span></span>

   <span data-ttu-id="ad865-113">\<DomainGUID\> yra `.mail.protection.outlook.com` pasirinktinio domeno tinkinto MX įrašo tekstas kairėje (pvz `contoso-com` ., domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ad865-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="ad865-114">\<InitialDomain\> yra domenas, kurį naudojote, kai prisiregistravote naudoti "Microsoft 365" (pvz., contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="ad865-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="ad865-115">Sukūrę CNAME įra us savo pasirinktiniams domenams, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="ad865-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="ad865-116">a.</span><span class="sxs-lookup"><span data-stu-id="ad865-116">a.</span></span> <span data-ttu-id="ad865-117">[Prisijunkite prie "Microsoft 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) naudodami savo darbo arba mokymo įstaigos paskyrą.</span><span class="sxs-lookup"><span data-stu-id="ad865-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="ad865-118">b.</span><span class="sxs-lookup"><span data-stu-id="ad865-118">b.</span></span> <span data-ttu-id="ad865-119">Pasirinkite taikomųjų programų vykdyklės piktogramą viršuje kairėje ir pasirinkite **administravimas**.</span><span class="sxs-lookup"><span data-stu-id="ad865-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="ad865-120">c.</span><span class="sxs-lookup"><span data-stu-id="ad865-120">c.</span></span> <span data-ttu-id="ad865-121">Apatinėje kairiojoje naršymo srityje išplėskite **administravimas** ir pasirinkite " **Exchange**".</span><span class="sxs-lookup"><span data-stu-id="ad865-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="ad865-122">d.</span><span class="sxs-lookup"><span data-stu-id="ad865-122">d.</span></span> <span data-ttu-id="ad865-123">Eikite į **apsaugos**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="ad865-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="ad865-124">e.</span><span class="sxs-lookup"><span data-stu-id="ad865-124">e.</span></span> <span data-ttu-id="ad865-125">Pasirinkite domeną, tada pasirinkite **įjungti** **šio domeno parašo pranešimą su DKIM parašais**.</span><span class="sxs-lookup"><span data-stu-id="ad865-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="ad865-126">Pakartokite šį veiksmą su kiekvienu pasirinktiniu domenu.</span><span class="sxs-lookup"><span data-stu-id="ad865-126">Repeat this step for each custom domain.</span></span>
