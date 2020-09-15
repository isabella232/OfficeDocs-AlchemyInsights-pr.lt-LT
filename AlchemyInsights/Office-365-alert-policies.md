---
title: 1385 – "Office" – "365" – įspėjimas – strategijos
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664034"
---
# <a name="alert-policies"></a><span data-ttu-id="96e37-102">Įspėjimų strategijos</span><span class="sxs-lookup"><span data-stu-id="96e37-102">Alert policies</span></span>

<span data-ttu-id="96e37-103">"Microsoft" 365 saugos & atitikties centras siūlo [numatytąsias įspėjimų strategijas](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) , kurios sukelia "Office 365 Enterprise" arba "Office 365 JAV Government" ("Office", "Office Enterprise" arba "Office", arba E5/G5 prenumeratos)</span><span class="sxs-lookup"><span data-stu-id="96e37-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="96e37-104">Todėl administratoriai gali gauti įspėjimų el. pašto pranešimus, atsiųstus "Office365Alerts@microsoft.com", naudojant temos eilutę, pvz., "žemas pavojingumo Įspėjimas: *įspėjimų strategijos pavadinimas*".</span><span class="sxs-lookup"><span data-stu-id="96e37-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="96e37-105">Įspėjimų pranešimai siunčiami, kai perspėjimai suaktyvinami dėl įprastinių veiksmų, pvz., kai vartotojai:</span><span class="sxs-lookup"><span data-stu-id="96e37-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="96e37-106">Sukurkite aplanko Gauta taisykles, kurios peradresuotų el. paštą.</span><span class="sxs-lookup"><span data-stu-id="96e37-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="96e37-107">Priskirkite teises savo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="96e37-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="96e37-108">Bendrinkite arba naikinkite didelį failų skaičių "SharePoint" failų bendrinimo programoje.</span><span class="sxs-lookup"><span data-stu-id="96e37-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="96e37-109">Kurti "Udiscovery" iešką ir eksportuoti ieškos rezultatus.</span><span class="sxs-lookup"><span data-stu-id="96e37-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="96e37-110">Norėdami peržiūrėti ir įjungti įspėjimą:</span><span class="sxs-lookup"><span data-stu-id="96e37-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="96e37-111">Eikite į [saugos & atitikties centrą](https://protection.office.com) ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="96e37-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="96e37-112">Spustelėkite **įspėjimų**rodymo  >  **įspėjimai**.</span><span class="sxs-lookup"><span data-stu-id="96e37-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="96e37-113">Spustelėkite įspėjimą, kad būtų rodomas Iškeliamasis puslapis su informacija apie įspėjimą.</span><span class="sxs-lookup"><span data-stu-id="96e37-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="96e37-114">Galite atlikti veiksmą su įspėjimu, pvz., [pašalinti įtartiną aplanko Gauta taisyklę](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="96e37-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="96e37-115">Arba galite tiesiog uždaryti įspėjimą spustelėdami **išspręsti** puslapyje perspėjimo Iškeliamasis puslapis.</span><span class="sxs-lookup"><span data-stu-id="96e37-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="96e37-116">Daugiau informacijos apie įspėjimų strategijų konfigūravimą ir valdymą rasite  [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="96e37-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="96e37-117">**Svarbu**: įspėjimų el. pašto pranešimai iš "Microsoft" niekada neprašo atlikti šių veiksmų:</span><span class="sxs-lookup"><span data-stu-id="96e37-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="96e37-118">Slaptažodžio pateikimas</span><span class="sxs-lookup"><span data-stu-id="96e37-118">Provide a password</span></span>
- <span data-ttu-id="96e37-119">Patikrinkite savo paskyros saugos duomenis</span><span class="sxs-lookup"><span data-stu-id="96e37-119">Verify the security details of your account</span></span>
- <span data-ttu-id="96e37-120">Pakartotinis savęs autentifikuoti</span><span class="sxs-lookup"><span data-stu-id="96e37-120">Re-authenticate yourself</span></span>

<span data-ttu-id="96e37-121">Jei gaunate tokį laišką, jis nebuvo išsiųstas "Microsoft" ir turėtų būti laikomas sukčiavimo apsimetant.</span><span class="sxs-lookup"><span data-stu-id="96e37-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="96e37-122">Jei taip nutiks, praneškite [apie tai "Microsoft"](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="96e37-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>