---
title: Nustatyti aplanko Gauta taisyklę veiklos audito žurnaluose
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417254"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="cec6e-102">Nustatyti aplanko Gauta taisyklę veiklos audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="cec6e-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="cec6e-103">Audito žurnalo paieška: į saugos & atitikties užtikrinimo centre galite peržiūrėti aplanko Gauta taisyklę įvykių (kurti, keisti ir ištrinti aplanko Gauta taisykles).</span><span class="sxs-lookup"><span data-stu-id="cec6e-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="cec6e-104">Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="cec6e-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="cec6e-105">Spustelėkite **paieškos ir tyrimas** ir pasirinkite **Audito žurnalo paieška**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="cec6e-106">Pasirinkite datos intervalą laukuose **pradžios data** ir **pabaigos data** .</span><span class="sxs-lookup"><span data-stu-id="cec6e-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="cec6e-107">**Exchange pašto dėžučių veikla**, patikrinkite, ar **veiklos** laukas yra nustatytas **New-InboxRule sukurti/keisti/įjungti/išjungti aplanko Gauta taisyklę**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="cec6e-108">Spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-108">Click **Search**.</span></span>

<span data-ttu-id="cec6e-109">Rezultatų sąraše pasirinkite audito įrašas.</span><span class="sxs-lookup"><span data-stu-id="cec6e-109">In the results, select an audit record.</span></span> <span data-ttu-id="cec6e-110">Detalių išskleidžiamojo meniu spustelėkite **Daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="cec6e-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="cec6e-111">**Parametrų** srityje rodoma informacija apie aplanko Gauta taisyklę parametrai.</span><span class="sxs-lookup"><span data-stu-id="cec6e-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="cec6e-112">Daugiau informacijos ieškokite [renkant jei vartotojo sukurti aplanko Gauta taisyklę](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="cec6e-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
