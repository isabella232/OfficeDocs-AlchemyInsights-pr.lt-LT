---
title: Klasikinės "SharePoint" audito žurnalo ataskaitos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509608"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="283d6-102">"SharePoint" ir "OneDrive" audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="283d6-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="283d6-103">"SharePoint" klasikiniai audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="283d6-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="283d6-104">SPO senstelėjusios įrangos auditas perkeltas į vieningąjį audito žurnalą (UAL).</span><span class="sxs-lookup"><span data-stu-id="283d6-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="283d6-105">Visos SPO senstelėjusios įrangos audito ataskaitos dabar bus parengtos per UAL, o senstelėjusios įrangos audito signalai perkelti į UAL.</span><span class="sxs-lookup"><span data-stu-id="283d6-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="283d6-106">Pagrindiniai pakeitimai:</span><span class="sxs-lookup"><span data-stu-id="283d6-106">Key changes:</span></span>

* <span data-ttu-id="283d6-107">Apipjaustymas nėra galimas kaip galimybė.</span><span class="sxs-lookup"><span data-stu-id="283d6-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="283d6-108">Konkrečių audito įvykių pasirinkimas negalimas.</span><span class="sxs-lookup"><span data-stu-id="283d6-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="283d6-109">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) ar nėra išsamaus audituotų įvykių sąrašo, kurį galima pasiekti pagal numatytuosius nustatymus.</span><span class="sxs-lookup"><span data-stu-id="283d6-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="283d6-110">Parinktis **Vieta** dalyje **Tinkintos ataskaitos** negalima.</span><span class="sxs-lookup"><span data-stu-id="283d6-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="283d6-111">Parinktis **Dokumentų atidarymo arba atsisiuntimo** įvykių atidaryti arba atsisiųsti negalima.</span><span class="sxs-lookup"><span data-stu-id="283d6-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="283d6-112">Svetainių rinkinio audito parametrų konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="283d6-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="283d6-113">"SharePoint" ir "OneDrive" šiuolaikinės vieningosios audito žurnalus iš atitikties</span><span class="sxs-lookup"><span data-stu-id="283d6-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="283d6-114">Įjungti / išjungti vieningąjį audito registravimą</span><span class="sxs-lookup"><span data-stu-id="283d6-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="283d6-115">"SharePoint" arba "OneDrive" nereikia papildomos konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="283d6-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="283d6-116">Naudokite audito registravimo iešką failo (-ų), aplanko (-ų), vartotojo (-ų), teisių veiklai tikrinti:</span><span class="sxs-lookup"><span data-stu-id="283d6-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="283d6-117">Failų ir puslapių veiklos</span><span class="sxs-lookup"><span data-stu-id="283d6-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="283d6-118">Aplanko veiklos</span><span class="sxs-lookup"><span data-stu-id="283d6-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="283d6-119">Užklausų veiklos bendrinimas ir prieiga prie jos</span><span class="sxs-lookup"><span data-stu-id="283d6-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="283d6-120">Sinchronizavimo veiklos</span><span class="sxs-lookup"><span data-stu-id="283d6-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="283d6-121">Svetainės administravimo veikla</span><span class="sxs-lookup"><span data-stu-id="283d6-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="283d6-122">Daugiau informacijos apie tai, kaip gauti šiuos įvykius, ieškokite [Audito žurnalo paieška](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="283d6-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
