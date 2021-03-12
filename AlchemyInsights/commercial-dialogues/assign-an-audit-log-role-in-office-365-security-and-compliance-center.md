---
title: Audito žurnalų vaidmens priskyrimas "Office 365" saugos & atitikties centre
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749516"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="8c33f-102">Audito žurnalų vaidmens priskyrimas "Office 365" saugos & atitikties centre</span><span class="sxs-lookup"><span data-stu-id="8c33f-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="8c33f-103">Norint ieškoti "Office 365" audito žurnale, administratoriui turi būti priskirtas **tik peržiūrėti audito žurnalų** vaidmuo arba **audito žurnalų** vaidmuo "Exchange Online".</span><span class="sxs-lookup"><span data-stu-id="8c33f-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="8c33f-104">Šie vaidmenys yra priskirti atitikties valdymo ir organizacijos valdymo vaidmenų grupėms pagal numatytuosius numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="8c33f-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="8c33f-105">Visuotinis "Office 365" ir "Microsoft 365" administratoriai automatiškai įtraukiami kaip organizacijos valdymo vaidmenų grupės nariai.</span><span class="sxs-lookup"><span data-stu-id="8c33f-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="8c33f-106">Norėdami įgalinti vartotoją ieškoti naudojant minimalų teisių lygį, sukurkite pasirinktinę vaidmenų grupę "Exchange Online", įtraukite **tik peržiūrėti skirtą audito žurnalų** vaidmenį arba **audito žurnalų** vaidmenį ir įtraukite vartotoją kaip naujos vaidmenų grupės narį.</span><span class="sxs-lookup"><span data-stu-id="8c33f-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="8c33f-107">Daugiau informacijos ieškokite [Vaidmenų grupių valdymas "Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) " ir [audito žurnalų ieška saugos & atitikties centre](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="8c33f-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>