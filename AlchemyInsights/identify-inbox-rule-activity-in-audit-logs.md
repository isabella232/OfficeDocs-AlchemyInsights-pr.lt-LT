---
title: Aplanko Gauta taisyklės veiklos identifikavimas audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779059"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ae497-102">Aplanko Gauta taisyklės veiklos identifikavimas audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="ae497-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ae497-103">Galite naudoti audito žurnalų iešką "Microsoft" 365 saugos & atitikties centre, kad peržiūrėtumėte aplanko Gauta taisyklės įvykius (kūrimo, modifikavimo ir naikinimo taisykles).</span><span class="sxs-lookup"><span data-stu-id="ae497-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ae497-104">Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ae497-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ae497-105">Eikite į puslapį **ieškos**  >  **audito žurnalų ieška** .</span><span class="sxs-lookup"><span data-stu-id="ae497-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ae497-106">Laukuose **pradžios data** ir **pabaigos data** pasirinkite datų intervalą.</span><span class="sxs-lookup"><span data-stu-id="ae497-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ae497-107">Dalyje " **Exchange" pašto dėžutės veikla**patikrinkite, ar laukas **veikla** nustatyta į **New-inboxtaisyklę kurti/modifikuoti/įjungti/išjungti aplanko Gauta taisyklę**.</span><span class="sxs-lookup"><span data-stu-id="ae497-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ae497-108">Spustelėkite **ieška**.</span><span class="sxs-lookup"><span data-stu-id="ae497-108">Click **Search**.</span></span>

<span data-ttu-id="ae497-109">Rezultatuose pasirinkite audito įrašą.</span><span class="sxs-lookup"><span data-stu-id="ae497-109">In the results, select an audit record.</span></span> <span data-ttu-id="ae497-110">Išsamios informacijos išskridimas spustelėkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="ae497-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ae497-111">Informacija apie aplanko Gauta taisyklės parametrus rodoma lauke **Parametrai** .</span><span class="sxs-lookup"><span data-stu-id="ae497-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ae497-112">Daugiau informacijos ieškokite kaip [nustatyti, ar vartotojas sukūrė aplanko Gauta taisyklę](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="ae497-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
