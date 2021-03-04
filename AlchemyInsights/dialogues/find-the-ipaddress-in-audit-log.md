---
title: IP adreso radimas audito logijoje
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429784"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="b59ef-102">IP adreso radimas audito logijoje</span><span class="sxs-lookup"><span data-stu-id="b59ef-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="b59ef-103">IP adresas, atitinkantis vartotojo arba administratoriaus vykdomą veiklą, rodomas audito žurnaluose.</span><span class="sxs-lookup"><span data-stu-id="b59ef-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="b59ef-104">Taip pat užregistruojamas kliento informacija.</span><span class="sxs-lookup"><span data-stu-id="b59ef-104">The client information is also logged.</span></span> <span data-ttu-id="b59ef-105">Štai kaip nustatyti IP adresą:</span><span class="sxs-lookup"><span data-stu-id="b59ef-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="b59ef-106">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="b59ef-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b59ef-107">Pasirinkite **ieškos**  >  **[audito žurnalų ieška](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="b59ef-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b59ef-108">Jei matote pranešimą, kad turite įjungti auditą, eikite į priekį ir įjunkite jį dabar.</span><span class="sxs-lookup"><span data-stu-id="b59ef-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="b59ef-109">Jei ši funkcija neįgalinta, ieškos rezultatai negalės ištraukti ankstesnių datų duomenų.</span><span class="sxs-lookup"><span data-stu-id="b59ef-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b59ef-110">Jei jus domina konkreti veikla, pasirinkite ją iš sąrašo **veikla** ; Priešingu atveju, pagal numatytuosius, visi veiksmai bus grąžinti pasirinktam vartotojui.</span><span class="sxs-lookup"><span data-stu-id="b59ef-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="b59ef-111">Atminkite, kad tam tikra veikla gali būti neprieinama pasirenkant meniu **veikla** ; Tačiau šie audito elementai bus pateikti, jei pažymėtas **visos veiklos rezultatų rodymas** (numatytasis parametras).</span><span class="sxs-lookup"><span data-stu-id="b59ef-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="b59ef-112">Nurodykite datų intervalą ir lauke **vartotojai** pasirinkite vartotojo, kurį norite tirti, vartotojo vardą.</span><span class="sxs-lookup"><span data-stu-id="b59ef-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="b59ef-113">Pasirinkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="b59ef-113">Select **Search**.</span></span> <span data-ttu-id="b59ef-114">Veikla rodoma dalyje **rezultatai**.</span><span class="sxs-lookup"><span data-stu-id="b59ef-114">The activities appear under **Results**.</span></span> <span data-ttu-id="b59ef-115">Galite peržiūrėti kiekvienos veiklos IP adresą.</span><span class="sxs-lookup"><span data-stu-id="b59ef-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="b59ef-116">Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="b59ef-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="b59ef-117">Norėdami sužinoti daugiau, skaitykite " [Office 365" audito žurnalų ieška, kad išspręstumėte įprastus scenarijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="b59ef-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>