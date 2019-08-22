---
title: Nustatyti IP adresą ir kliento audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539037"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="d8c3a-102">Nustatyti IP adresą ir kliento audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="d8c3a-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="d8c3a-103">IP adresą, kuris atitinka "Office 365" vartotojo ar administratoriaus veikla yra nurodyta audito žurnalus.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="d8c3a-104">Taip pat registruojamas kliento informacija.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-104">The client information is also logged.</span></span> <span data-ttu-id="d8c3a-105">Atlikite šiuos veiksmus, siekiant nustatyti tokią informaciją</span><span class="sxs-lookup"><span data-stu-id="d8c3a-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="d8c3a-106">Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d8c3a-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d8c3a-107">Grįžti į **paieškos** > **audito žurnalo paieškos** puslapyje.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="d8c3a-108">Jei jus domina konkrečiai veiklai, pasirinkite jį iš **veiklos** sąraše.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="d8c3a-109">Jei ne, visa veikla bus grąžintas iš pasirinkto vartotojo (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="d8c3a-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="d8c3a-110">**Pastaba**: tam tikra veikla gali būti prieinama meniu **veiklos** ; vis dėlto šie audito elementai bus grąžintas, jei **Rodyti rezultatus visoms veiklos rūšims** yra pasirinktas (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="d8c3a-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="d8c3a-111">**Vartotojams** lauke nurodykite vartotojo vardą, pasirinkite atitinkamą dienų seką veiklos, ir tada spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="d8c3a-112">Rezultatuose matote IP adresą šios veiklos rezultatų srityje.</span><span class="sxs-lookup"><span data-stu-id="d8c3a-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="d8c3a-113">Pasirinkite audito įrašą, norėdami pamatyti išsamią informaciją **detalių** flyout (pvz., klientas, vartotojas, kuris atliekamas veiksmas, ir kt.).</span><span class="sxs-lookup"><span data-stu-id="d8c3a-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="d8c3a-114">Norėdami gauti daugiau informacijos, peržiūrėkite [rasti IP adresą, kompiuteryje, kuris naudojamas gauti sugadintos paskyros](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="d8c3a-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
