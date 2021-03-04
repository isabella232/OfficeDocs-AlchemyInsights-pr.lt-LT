---
title: Panaikintų įvykių audito žurnalų skaitymas
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429829"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="dba08-102">Panaikintų įvykių audito žurnalų skaitymas</span><span class="sxs-lookup"><span data-stu-id="dba08-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="dba08-103">Štai kaip tai padaryti:</span><span class="sxs-lookup"><span data-stu-id="dba08-103">Here's how to do this:</span></span>

1. <span data-ttu-id="dba08-104">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="dba08-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="dba08-105">Pasirinkite **ieškos**  >  [**audito žurnalų ieška**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="dba08-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="dba08-106">Jei matote pranešimą, kad norite įjungti funkciją, eikite į priekį ir įjunkite ją dabar.</span><span class="sxs-lookup"><span data-stu-id="dba08-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="dba08-107">Jei funkcija neįjungta, ieškos rezultatai negalės ištraukti ankstesnių datų duomenų.</span><span class="sxs-lookup"><span data-stu-id="dba08-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="dba08-108">Pasirinkite **veikla**, tada Raskite " **Exchange" pašto dėžutės veiklas**.</span><span class="sxs-lookup"><span data-stu-id="dba08-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="dba08-109">Pažymėkite **panaikintus laiškus iš aplanko panaikinta** ir **perkėlėte laiškus į panaikintų elementų** aplanko parinktis.</span><span class="sxs-lookup"><span data-stu-id="dba08-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="dba08-110">Kai baigsite, spustelėkite už srities ribų, kad sumažintumėte **veiklos** sritį.</span><span class="sxs-lookup"><span data-stu-id="dba08-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="dba08-111">Nurodykite datų intervalą, tada lauke **vartotojai** pasirinkite vartotojo, kurį norite tirti, vartotojo vardą.</span><span class="sxs-lookup"><span data-stu-id="dba08-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="dba08-112">Vienu metu galite pasirinkti daugiau nei vieną vartotoją.</span><span class="sxs-lookup"><span data-stu-id="dba08-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="dba08-113">Pasirinkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="dba08-113">Select **Search**.</span></span> <span data-ttu-id="dba08-114">Veikla rodoma dalyje **rezultatai**.</span><span class="sxs-lookup"><span data-stu-id="dba08-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="dba08-115">Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="dba08-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="dba08-116">Papildoma informacija apie panaikintą elementą, pvz., temos eilutę ir elemento vietą, kai jis buvo panaikintas, rodoma lauke **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="dba08-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="dba08-117">Negalite atkurti panaikintų elementų naudodami audito žurnalų funkciją.</span><span class="sxs-lookup"><span data-stu-id="dba08-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="dba08-118">Norėdami atkurti panaikintus elementus, skaitykite [panaikintų elementų arba laiškų atkūrimas "Outlook Web App"](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="dba08-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="dba08-119">Norėdami sužinoti daugiau, skaitykite " [Office 365" audito žurnalų ieška, kad išspręstumėte įprastus scenarijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="dba08-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
