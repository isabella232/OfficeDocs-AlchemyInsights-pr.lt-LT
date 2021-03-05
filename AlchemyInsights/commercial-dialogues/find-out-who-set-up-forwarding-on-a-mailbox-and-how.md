---
title: Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482302"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="8732c-102">Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip</span><span class="sxs-lookup"><span data-stu-id="8732c-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="8732c-103">Jei išorinis peradresavimas buvo nustatytas pašto dėžutėje, veikla tikrinama kaip Set-Mailbox cmdlet dalis.</span><span class="sxs-lookup"><span data-stu-id="8732c-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="8732c-104">Toliau aprašyta, kaip galite sužinoti veiklos auditą:</span><span class="sxs-lookup"><span data-stu-id="8732c-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="8732c-105">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="8732c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="8732c-106">Pasirinkite **ieškos** >  **audito žurnalų ieška**.</span><span class="sxs-lookup"><span data-stu-id="8732c-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="8732c-107">Jei matote pranešimą, kad turite įjungti auditą, eikite į priekį ir įjunkite jį dabar.</span><span class="sxs-lookup"><span data-stu-id="8732c-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="8732c-108">Jei ši funkcija nėra įjungta, ieškos rezultatai negalės ištraukti ankstesnių datų duomenų.</span><span class="sxs-lookup"><span data-stu-id="8732c-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="8732c-109">Įsitikinkite, kad lauke **veikla** nustatyta **Rodyti visų veiklų rezultatus** (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="8732c-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="8732c-110">Nurodo datų intervalą.</span><span class="sxs-lookup"><span data-stu-id="8732c-110">Specify the date range.</span></span> <span data-ttu-id="8732c-111">Jums nereikia įvesti vartotojo vardo.</span><span class="sxs-lookup"><span data-stu-id="8732c-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="8732c-112">Pasirinkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="8732c-112">Select **Search**.</span></span> <span data-ttu-id="8732c-113">Veikla rodoma dalyje **rezultatai**.</span><span class="sxs-lookup"><span data-stu-id="8732c-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="8732c-114">Pasirinkite **filtruoti rezultatus**, tada lauke **veiklos** filtras įveskite **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="8732c-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="8732c-115">Tai pateikia visas **nustatytas pašto dėžutės** veiklas.</span><span class="sxs-lookup"><span data-stu-id="8732c-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="8732c-116">Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="8732c-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="8732c-117">Dalyje **Parametrai** galite matyti peradresavimo el. pašto adresą, kuris buvo nustatytas pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="8732c-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="8732c-118">**UserID** vaizduoja vartotoją, kuris nustatė išorinį peradresavimą pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="8732c-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="8732c-119">Norėdami sužinoti daugiau, skaitykite " [Office 365" audito žurnalų ieška, kad išspręstumėte įprastus scenarijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="8732c-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>