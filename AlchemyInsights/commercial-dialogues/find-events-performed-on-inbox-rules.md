---
title: Aplanko Gauta taisyklių radimo įvykiai
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482600"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="be0c8-102">Aplanko Gauta taisyklių radimo įvykiai</span><span class="sxs-lookup"><span data-stu-id="be0c8-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="be0c8-103">Kai aplanko Gauta taisyklės sukurtos, pakeistos arba panaikintos, įvykiai įrašomi į audito žurnalų.</span><span class="sxs-lookup"><span data-stu-id="be0c8-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="be0c8-104">Štai kaip juos peržiūrėti:</span><span class="sxs-lookup"><span data-stu-id="be0c8-104">Here's how to review them:</span></span>

1. <span data-ttu-id="be0c8-105">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="be0c8-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="be0c8-106">Pasirinkite ieškoti > audito žurnalų ieška.</span><span class="sxs-lookup"><span data-stu-id="be0c8-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="be0c8-107">Jei matote pranešimą, kad turite įjungti auditą, eikite į priekį ir įjunkite jį dabar.</span><span class="sxs-lookup"><span data-stu-id="be0c8-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="be0c8-108">Jei ši funkcija nėra įjungta, ieškos rezultatai negalės ištraukti ankstesnių datų duomenų.</span><span class="sxs-lookup"><span data-stu-id="be0c8-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="be0c8-109">Pasirinkite veiklos lauką ir raskite "Exchange" pašto dėžutės veiklas, tada pasirinkite New-InboxRule kurti aplanko Gauta taisyklę iš "Outlook Web App".</span><span class="sxs-lookup"><span data-stu-id="be0c8-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="be0c8-110">Kai baigsite, spustelėkite už srities ribų, kad sumažintumėte veiklos sritį.</span><span class="sxs-lookup"><span data-stu-id="be0c8-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="be0c8-111">Nurodykite datų intervalą, tada lauke vartotojai pasirinkite vartotojo, kurį norite tirti, vartotojo vardą.</span><span class="sxs-lookup"><span data-stu-id="be0c8-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="be0c8-112">Vienu metu galite pasirinkti daugiau nei vieną vartotoją.</span><span class="sxs-lookup"><span data-stu-id="be0c8-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="be0c8-113">Pasirinkite Ieškoti.</span><span class="sxs-lookup"><span data-stu-id="be0c8-113">Select Search.</span></span> <span data-ttu-id="be0c8-114">Veikla rodoma dalyje rezultatai.</span><span class="sxs-lookup"><span data-stu-id="be0c8-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="be0c8-115">Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="be0c8-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="be0c8-116">Dalyje Parametrai galite matyti taisyklės pavadinimą, nustatytas sąlygas ir veiksmus, kurių imsis taisyklė.</span><span class="sxs-lookup"><span data-stu-id="be0c8-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="be0c8-117">Norėdami sužinoti daugiau, skaitykite "Office 365" audito žurnalų ieška, kad išspręstumėte įprastus scenarijus.</span><span class="sxs-lookup"><span data-stu-id="be0c8-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>