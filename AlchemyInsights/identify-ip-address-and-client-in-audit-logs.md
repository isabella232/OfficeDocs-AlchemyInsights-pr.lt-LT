---
title: IP adreso ir kliento identifikavimas audito žurnaluose
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668318"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="b0e14-102">IP adreso ir kliento identifikavimas audito žurnaluose</span><span class="sxs-lookup"><span data-stu-id="b0e14-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="b0e14-103">IP adresas, atitinkantis "Microsoft" 365 vartotojo arba administratoriaus veiklą, rodomas audito žurnaluose.</span><span class="sxs-lookup"><span data-stu-id="b0e14-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="b0e14-104">Taip pat užregistruojamas kliento informacija.</span><span class="sxs-lookup"><span data-stu-id="b0e14-104">The client information is also logged.</span></span> <span data-ttu-id="b0e14-105">Toliau pateikiami tokios informacijos nustatymo veiksmai</span><span class="sxs-lookup"><span data-stu-id="b0e14-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="b0e14-106">Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b0e14-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="b0e14-107">Eikite į puslapį **ieškos**  >  **audito žurnalų ieška** .</span><span class="sxs-lookup"><span data-stu-id="b0e14-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="b0e14-108">Jei jus domina konkreti veikla, pasirinkite ją iš sąrašo **veikla** .</span><span class="sxs-lookup"><span data-stu-id="b0e14-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="b0e14-109">Jei ne, visos veiklos bus grąžintos pasirinktam vartotojui (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="b0e14-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="b0e14-110">**Pastaba**: tam tikra veikla gali būti neprieinama meniu **veikla** ; Tačiau šie audito elementai bus pateikti, jei pažymėtas **visos veiklos rezultatų rodymas** (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="b0e14-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="b0e14-111">Nurodykite vartotojo vardą lauke **vartotojai** , pasirinkite reikiamą veiklos datų intervalą ir spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="b0e14-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="b0e14-112">Rezultatuose galite matyti tos veiklos IP adresą rezultatų srityje.</span><span class="sxs-lookup"><span data-stu-id="b0e14-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="b0e14-113">Pasirinkite audito įrašą, kad pamatytumėte išsamią **informaciją išsamios informacijos** iškeliamojo (pvz., kliento, vartotojo, kuris atliko veiksmą ir kt.).</span><span class="sxs-lookup"><span data-stu-id="b0e14-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="b0e14-114">Daugiau informacijos ieškokite kompiuterio, [naudojamo pasiekti kompromisinį abonementą, IP adreso radimas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="b0e14-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
