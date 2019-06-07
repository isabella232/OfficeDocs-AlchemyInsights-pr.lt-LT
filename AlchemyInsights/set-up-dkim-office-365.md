---
title: DKIM "Office 365" sąranka
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765253"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="6aa09-102">DKIM "Office 365" sąranka</span><span class="sxs-lookup"><span data-stu-id="6aa09-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="6aa09-103">Visą instrukciją konfigūravimo DKIM pasirinktinius domenus "Office 365" yra [čia](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6aa09-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="6aa09-104">**Kiekvieno** vartotojo domeno, turite sukurti **du** DKIM CNAME įrašus ne savo domeno DNS išteklių nuomos tarnybą (paprastai, domenų registratorius).</span><span class="sxs-lookup"><span data-stu-id="6aa09-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="6aa09-105">Pvz., contoso.com ir fourthcoffee.com reikia keturių DKIM CNAME įra us: du contoso.com ir du fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="6aa09-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="6aa09-106">DKIM CNAME įrašus apie **kiekvieno** individualiame domene naudoti šiuos formatus:</span><span class="sxs-lookup"><span data-stu-id="6aa09-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="6aa09-107">**Pagrindinio kompiuterio vardas**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6aa09-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6aa09-108">**Atkreipia dėmesį į adresą arba vertė**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6aa09-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6aa09-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6aa09-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="6aa09-110">**Pagrindinio kompiuterio vardas**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="6aa09-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="6aa09-111">**Atkreipia dėmesį į adresą arba vertė**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="6aa09-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="6aa09-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="6aa09-112">**TTL**: 3600</span></span>

   <span data-ttu-id="6aa09-113">\<DomainGUID\> -tekstas kairėje `.mail.protection.outlook.com` į individualų pasirinktinio domeno MX įrašas (pavyzdžiui, `contoso-com` už domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6aa09-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="6aa09-114">\<InitialDomain\> yra domenas, kurį naudojote, kai prisiregistravote prie "Office 365" (pvz., contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="6aa09-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="6aa09-115">Sukūrę CNAME įra us Pasirinktinių domenų, atlikite šiuos nurodymus:</span><span class="sxs-lookup"><span data-stu-id="6aa09-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="6aa09-116">a.</span><span class="sxs-lookup"><span data-stu-id="6aa09-116">a.</span></span> <span data-ttu-id="6aa09-117">[Prisijunkite prie "Office 365"](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) su savo darbovietės ar mokyklos paskyros.</span><span class="sxs-lookup"><span data-stu-id="6aa09-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="6aa09-118">b.</span><span class="sxs-lookup"><span data-stu-id="6aa09-118">b.</span></span> <span data-ttu-id="6aa09-119">Pasirinkite programos paleidimo piktograma viršutiniame kairiajame ir **administratorius**.</span><span class="sxs-lookup"><span data-stu-id="6aa09-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="6aa09-120">c.</span><span class="sxs-lookup"><span data-stu-id="6aa09-120">c.</span></span> <span data-ttu-id="6aa09-121">Apatiniame kairiajame naršymo, išplėskite **Admin** ir pasirinkite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="6aa09-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="6aa09-122">d.</span><span class="sxs-lookup"><span data-stu-id="6aa09-122">d.</span></span> <span data-ttu-id="6aa09-123">Eikite į **saugos** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="6aa09-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="6aa09-124">e.</span><span class="sxs-lookup"><span data-stu-id="6aa09-124">e.</span></span> <span data-ttu-id="6aa09-125">Pasirinkite domeno, tada pasirinkite **įjungti** pranešimams **pasirašyti šio domeno su DKIM parašais**.</span><span class="sxs-lookup"><span data-stu-id="6aa09-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="6aa09-126">Pakartokite šį veiksmą kiekvienam individualiame domene.</span><span class="sxs-lookup"><span data-stu-id="6aa09-126">Repeat this step for each custom domain.</span></span>
