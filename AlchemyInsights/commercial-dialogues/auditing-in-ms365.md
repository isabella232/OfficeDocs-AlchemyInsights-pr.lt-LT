---
title: "\"Microsoft 365\" tikrinimas"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482363"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="9fdfe-102">"Microsoft 365" tikrinimas</span><span class="sxs-lookup"><span data-stu-id="9fdfe-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="9fdfe-103">Štai keletas dalykų, kuriuos turėtumėte žinoti apie "Microsoft 365" auditą:</span><span class="sxs-lookup"><span data-stu-id="9fdfe-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="9fdfe-104">"Exchange" administravimo veikla yra tikrinama pagal numatytuosius numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="9fdfe-105">Mes apdorojame pašto dėžučių tikrinimo pagal numatytuosius numatytuosius ir visiems vartotojams procesą.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="9fdfe-106">Norėdami sužinoti daugiau apie tai, spustelėkite [čia](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span><span class="sxs-lookup"><span data-stu-id="9fdfe-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="9fdfe-107">Iki tada, jei norite, kad nurodymai būtų neautomatiškai įgalinti vienam žmogui arba visai organizacijai, pasirinkite toliau esantį mygtuką įjungti pašto dėžutės tikrinimą.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="9fdfe-108">"Microsoft" 365 grupių pašto dėžutės ir viešųjų aplankų pašto dėžutės nepalaiko audito registravimo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="9fdfe-109">"SharePoint"/"OneDrive" nėra papildomo konfigūravimo, reikalingo norint įgalinti tikrinimą.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="9fdfe-110">Norėdami sužinoti, kokia veikla tikrinama, žiūrėkite:</span><span class="sxs-lookup"><span data-stu-id="9fdfe-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="9fdfe-111">Failų veikla</span><span class="sxs-lookup"><span data-stu-id="9fdfe-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="9fdfe-112">Aplanko veikla</span><span class="sxs-lookup"><span data-stu-id="9fdfe-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="9fdfe-113">[Dalinimosi ir prieigos veikla](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span><span class="sxs-lookup"><span data-stu-id="9fdfe-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="9fdfe-114">Visų audituotų veiksmų pagal tarnybos sąrašą ieškokite straipsnyje [audituota veikla](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="9fdfe-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
