---
title: Klasikinės "SharePoint" audito žurnalo ataskaitos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992626"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="c0b0d-102">"SharePoint" ir "OneDrive" audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="c0b0d-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="c0b0d-103">SharePoint Classic audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="c0b0d-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="c0b0d-104">Į vieningosios audito žurnalą (UAL) perkeltas SPO palikimas auditas.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="c0b0d-105">Dabar visos SPO senstelėjusios įrangos audito ataskaitos bus maitinamas per UAL, o senstelėjusios įrangos audito signalai buvo perkelti į UAL.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="c0b0d-106">Pagrindiniai pakeitimai:</span><span class="sxs-lookup"><span data-stu-id="c0b0d-106">Key changes:</span></span>

* <span data-ttu-id="c0b0d-107">Apipjaustymas nėra galimybės.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="c0b0d-108">Pasirinkti konkrečius įvykius, kurių auditas yra neprieinamas.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="c0b0d-109">[Šiame dokumente](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) rasite visą audituotų renginių, kuriuos galima gauti pagal numatytuosius nustatymus, sąrašą.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="c0b0d-110">**Vietos** parinktis pagal **PRITAIKYTAS ataskaitas** yra neprieinama.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="c0b0d-111">Parinktis **atidaryti arba atsisiųsti dokumentus** įvykiai yra neprieinama.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="c0b0d-112">Konfigūruoti svetainių rinkinio audito parametrus</span><span class="sxs-lookup"><span data-stu-id="c0b0d-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="c0b0d-113">"SharePoint" ir "OneDrive" šiuolaikinės vieningosios audito žurnalai atitikties</span><span class="sxs-lookup"><span data-stu-id="c0b0d-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="c0b0d-114">Įjungti/išjungti vieningosios audito registravimą</span><span class="sxs-lookup"><span data-stu-id="c0b0d-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="c0b0d-115">"SharePoint" arba "OneDrive" nereikia papildomos konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="c0b0d-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="c0b0d-116">Naudokite audito registravimo iešką Norėdami patikrinti failo (-ų), aplanko (-ų), vartotojo (-ų), leidimų veiklą:</span><span class="sxs-lookup"><span data-stu-id="c0b0d-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="c0b0d-117">Failų ir puslapių veikla</span><span class="sxs-lookup"><span data-stu-id="c0b0d-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="c0b0d-118">Aplanko veikla</span><span class="sxs-lookup"><span data-stu-id="c0b0d-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="c0b0d-119">Bendrinimo ir prieigos užklausų veikla</span><span class="sxs-lookup"><span data-stu-id="c0b0d-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="c0b0d-120">Sinchronizavimo veikla</span><span class="sxs-lookup"><span data-stu-id="c0b0d-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="c0b0d-121">Svetainės administravimo veikla</span><span class="sxs-lookup"><span data-stu-id="c0b0d-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="c0b0d-122">Daugiau informacijos apie tai, kaip nuskaityti šiuos įvykius, rasite [Ieškoti audito žurnale](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="c0b0d-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
