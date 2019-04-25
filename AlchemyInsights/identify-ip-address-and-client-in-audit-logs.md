---
title: Nustatyti IP adresą ir kliento audito žurnaluose
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416995"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="cb26c-102">Nustatyti IP adresą ir kliento audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="cb26c-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="cb26c-103">IP adresą, kuris atitinka vartotojo ar administratoriaus veikla yra nurodyta audito žurnalus.</span><span class="sxs-lookup"><span data-stu-id="cb26c-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="cb26c-104">Taip pat registruojamas kliento informacija.</span><span class="sxs-lookup"><span data-stu-id="cb26c-104">The client information is also logged.</span></span> <span data-ttu-id="cb26c-105">Atlikite šiuos veiksmus, siekiant nustatyti tokią informaciją</span><span class="sxs-lookup"><span data-stu-id="cb26c-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="cb26c-106">Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="cb26c-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="cb26c-107">Spustelėkite **paieškos ir tyrimas** ir pasirinkite **Audito žurnalo paieška**.</span><span class="sxs-lookup"><span data-stu-id="cb26c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="cb26c-108">Jei jus domina konkrečiai veiklai, pasirinkite jį iš **veiklos** sąraše.</span><span class="sxs-lookup"><span data-stu-id="cb26c-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="cb26c-109">Jei ne, visa veikla bus grąžintas iš pasirinkto vartotojo (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="cb26c-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="cb26c-110">**Pastaba**: tam tikra veikla gali būti prieinama meniu **veiklos** ; vis dėlto šie audito elementai bus grąžintas, jei **Rodyti rezultatus visoms veiklos rūšims** yra pasirinktas (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="cb26c-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="cb26c-111">**Vartotojams** lauke nurodykite vartotojo vardą, pasirinkite atitinkamą dienų seką veiklos, ir tada spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="cb26c-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="cb26c-112">Rezultatuose matote IP adresą šios veiklos rezultatų srityje.</span><span class="sxs-lookup"><span data-stu-id="cb26c-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="cb26c-113">Pasirinkite audito įrašą, norėdami pamatyti išsamią informaciją **detalių** flyout (pvz., klientas, vartotojas, kuris atliekamas veiksmas, ir kt.).</span><span class="sxs-lookup"><span data-stu-id="cb26c-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="cb26c-114">Norėdami gauti daugiau informacijos, peržiūrėkite [rasti IP adresą, kompiuteryje, kuris naudojamas gauti sugadintos paskyros](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="cb26c-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
