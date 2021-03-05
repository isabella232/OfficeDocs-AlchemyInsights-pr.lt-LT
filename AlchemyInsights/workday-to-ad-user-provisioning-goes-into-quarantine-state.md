---
title: Darbo diena su skelbimo vartotojo parengimas pereina į sulaikytą būseną
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481879"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="f12ee-102">Darbo diena su skelbimo vartotojo parengimas pereina į sulaikytą būseną</span><span class="sxs-lookup"><span data-stu-id="f12ee-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="f12ee-103">**Darbo diena su skelbimo vartotojo parengimas patenka į sulaikytą būseną, o AD nėra kuriami jokie vartotojai**</span><span class="sxs-lookup"><span data-stu-id="f12ee-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="f12ee-104">Darbo dienos į skelbimų vartotojo parengimo užduotį atvyko į karantiną ir audito žurnalai rodo eksportavimo triktis su klaidos pranešimo **klaida: OperationsError-SvcErr: įvyko operacijos klaida. Katalogo tarnybai nesukonfigūruota aukštesnioji nuoroda. Todėl katalogų tarnyba negali perduoti klausimų į objektus, esančius už šio miško ribų**.</span><span class="sxs-lookup"><span data-stu-id="f12ee-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="f12ee-105">Ši klaida paprastai rodoma, jei "Active Directory" talpyklos OU nustatyta netinkamai arba kyla problemų dėl išraiškos priskyrimo, naudojamo su " **Parentatshed" pavadinimu**.</span><span class="sxs-lookup"><span data-stu-id="f12ee-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="f12ee-106">Pažymėkite žymės langelį numatytoji OU naujiems **vartotojams** .</span><span class="sxs-lookup"><span data-stu-id="f12ee-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="f12ee-107">Įsitikinkite, kad jūsų skelbime jau yra nurodyta OU.</span><span class="sxs-lookup"><span data-stu-id="f12ee-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="f12ee-108">Jei atributo **Atvaizdelyje naudojate Parentasshedname** , įsitikinkite, kad ji visada įvertinama kaip žinomas talpyklos, esančios skelbimo domene, konteineris.</span><span class="sxs-lookup"><span data-stu-id="f12ee-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="f12ee-109">Patikrinkite eksportavimo įvykį audito žurnaluose, kad pamatytumėte sugeneruotą reikšmę.</span><span class="sxs-lookup"><span data-stu-id="f12ee-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="f12ee-110">Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="f12ee-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

