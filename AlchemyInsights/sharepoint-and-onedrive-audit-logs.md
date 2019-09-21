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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068031"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="e9458-102">"SharePoint" ir "OneDrive" audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="e9458-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="e9458-103">**"SharePoint" ir "OneDrive" šiuolaikinės vieningosios audito žurnalai atitikties**</span><span class="sxs-lookup"><span data-stu-id="e9458-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="e9458-104">Įjungti/išjungti vieningosios audito registravimą</span><span class="sxs-lookup"><span data-stu-id="e9458-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="e9458-105">"SharePoint" arba "OneDrive" nereikia papildomos konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="e9458-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="e9458-106">Naudokite audito registravimo iešką Norėdami patikrinti failo (-ų), aplanko (-ų), vartotojo (-ų), leidimų veiklą:</span><span class="sxs-lookup"><span data-stu-id="e9458-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="e9458-107">Failų ir puslapių veikla</span><span class="sxs-lookup"><span data-stu-id="e9458-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="e9458-108">Aplanko veikla</span><span class="sxs-lookup"><span data-stu-id="e9458-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="e9458-109">Bendrinimo ir prieigos užklausų veikla</span><span class="sxs-lookup"><span data-stu-id="e9458-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="e9458-110">Sinchronizavimo veikla</span><span class="sxs-lookup"><span data-stu-id="e9458-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="e9458-111">Svetainės administravimo veikla</span><span class="sxs-lookup"><span data-stu-id="e9458-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="e9458-112">Daugiau informacijos apie tai, kaip nuskaityti šiuos įvykius, rasite [Ieškoti audito žurnale](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="e9458-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="e9458-113">**SharePoint Classic audito žurnalai**</span><span class="sxs-lookup"><span data-stu-id="e9458-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="e9458-114">Perkelėme SPO palikimą į vieningosios audito žurnalo (UAL) auditą.</span><span class="sxs-lookup"><span data-stu-id="e9458-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="e9458-115">Tai iš esmės reiškia, kad dabar visos SPO senstelėjusios įrangos audito ataskaitos bus maitinamas per UAL, o senesni audito signalai buvo perkelti į UAL.</span><span class="sxs-lookup"><span data-stu-id="e9458-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="e9458-116">Pagrindiniai pakeitimai:</span><span class="sxs-lookup"><span data-stu-id="e9458-116">Key changes:</span></span>

- <span data-ttu-id="e9458-117">NEGALIMA apipjaustyti kaip galimybės.</span><span class="sxs-lookup"><span data-stu-id="e9458-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="e9458-118">Sekcija, kurioje pasirenkate konkrečius audito įvykius, yra neprieinama.</span><span class="sxs-lookup"><span data-stu-id="e9458-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="e9458-119">Prašome kreiptis į [šį dokumentą](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) visą audituotų renginių, galimų pagal numatytuosius nustatymus, sąrašą.</span><span class="sxs-lookup"><span data-stu-id="e9458-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="e9458-120">Parinktis "vieta" pagal **pritaikytas ataskaitas** yra neprieinama.</span><span class="sxs-lookup"><span data-stu-id="e9458-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="e9458-121">"Dokumentų atidarymas arba atsisiuntimas" įvykiai nepasiekiami.</span><span class="sxs-lookup"><span data-stu-id="e9458-121">“Opening or downloading documents” events is NOT available.</span></span> 

