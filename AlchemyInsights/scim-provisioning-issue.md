---
title: SCIM parengimo problema
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949941"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="660e3-102">SCIM parengimo problema</span><span class="sxs-lookup"><span data-stu-id="660e3-102">SCIM provisioning issue</span></span>

<span data-ttu-id="660e3-103">Automatinis parengimas reiškia vartotojų tapatybių kūrimą ir vaidmenis debesyje taikomosiose programose, prie kurių vartotojai turi prieigą.</span><span class="sxs-lookup"><span data-stu-id="660e3-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="660e3-104">Be vartotojų tapatybių kūrimo, automatinis parengimas yra vartotojo tapatybių išlaikymas ir pašalinimas kaip būsena arba vaidmenys.</span><span class="sxs-lookup"><span data-stu-id="660e3-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="660e3-105">Prieš pradėdami diegti, galite peržiūrėti, kaip veikia [parengimas](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) , kad sužinotumėte, kaip veikia "Azure Active Directory" (skelbimų) nuostata, ir gaukite konfigūravimo rekomendacijų.</span><span class="sxs-lookup"><span data-stu-id="660e3-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="660e3-106">Kaip taikomųjų programų kūrėjas, galite naudoti kelių domenų tapatybės valdymo (SCIM) vartotojų valdymo API sistemą, kad įgalintumėte automatinį vartotojų ir grupių parengimą tarp taikomosios programos ir "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="660e3-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="660e3-107">[Kuriant "SCIM" galinį punktą ir konfigūruojant vartotojo parengimą su "AZURE ad](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) ", aprašoma, kaip kurti "SCIM" galinį punktą ir integruoti jį su "Azure AD" parengimo tarnyba.</span><span class="sxs-lookup"><span data-stu-id="660e3-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



