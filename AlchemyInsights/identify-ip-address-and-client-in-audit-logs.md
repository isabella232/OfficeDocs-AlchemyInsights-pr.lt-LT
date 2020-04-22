---
title: Nustatyti IP adresą ir kliento audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716396"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="041cc-102">Nustatyti IP adresą ir kliento audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="041cc-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="041cc-103">IP adresas, kuris atitinka "Microsoft 365" vartotojo arba administratoriaus veiklą, rodomas audito žurnaluose.</span><span class="sxs-lookup"><span data-stu-id="041cc-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="041cc-104">Kliento informacija taip pat užregistruojamas.</span><span class="sxs-lookup"><span data-stu-id="041cc-104">The client information is also logged.</span></span> <span data-ttu-id="041cc-105">Toliau pateikiami veiksmai, kaip nustatyti tokią informaciją</span><span class="sxs-lookup"><span data-stu-id="041cc-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="041cc-106">Prisijunkite prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="041cc-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="041cc-107">Eikite į **ieškos** > **tikrinimo žurnalo ieškos** puslapį.</span><span class="sxs-lookup"><span data-stu-id="041cc-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="041cc-108">Jei jus domina konkreti veikla, pasirinkite ją iš **sąrašo Veikla.**</span><span class="sxs-lookup"><span data-stu-id="041cc-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="041cc-109">Jei ne, bus grąžintos visos pasirinkto vartotojo veiklos (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="041cc-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="041cc-110">**Pastaba:** meniu **Veikla** gali nebūti tam tikros veiklos; tačiau šios audito prekės bus grąžintos, jei bus pasirinkti **Rodyti visų veiklų rezultatus** (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="041cc-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="041cc-111">Lauke **Vartotojai** nurodykite vartotojo vardą, pasirinkite atitinkamą veiklos dienų seką ir spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="041cc-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="041cc-112">Rezultatuose rezultatų srityje galite matyti tos veiklos IP adresą.</span><span class="sxs-lookup"><span data-stu-id="041cc-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="041cc-113">Pasirinkite audito įrašą, kad pamatytumėte išsamią informaciją **iškeliamame** pranešime (pvz., Klientas, Vartotojas, kuris atliko veiksmą ir t. t.).</span><span class="sxs-lookup"><span data-stu-id="041cc-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="041cc-114">Daugiau informacijos [ieškokite Kompiuterio, naudojamo norint pasiekti pažeistą abonementą, IP adreso radimas](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="041cc-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
