---
title: Nustatyti ištrinti pranešimą įvykių audito žurnalai
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909401"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="df5c5-102">Audito žurnalų panaikintus el. laiškus</span><span class="sxs-lookup"><span data-stu-id="df5c5-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="df5c5-103">Nuo 2019 m. sausio, "Microsoft" įjungti pašto dėžutės audito žurnalų pagal numatytuosius nustatymus.</span><span class="sxs-lookup"><span data-stu-id="df5c5-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="df5c5-104">Priešingu atveju peržiūrėti ištrinti pranešimą įvykių skirtas konkrečiam vartotojui, jums reikia rankiniu būdu įgalinti ištrinti veiksmus auditas.</span><span class="sxs-lookup"><span data-stu-id="df5c5-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="df5c5-105">Jei pašto dėžutės audito registravimo jau įjungtas jūsų organizacijoje arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="df5c5-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="df5c5-106">Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="df5c5-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="df5c5-107">Spustelėkite **paieškos ir tyrimas** ir pasirinkite **Audito žurnalo paieška**.</span><span class="sxs-lookup"><span data-stu-id="df5c5-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="df5c5-108">Pasirinkite datos intervalą laukuose **pradžios data** ir **pabaigos data** .</span><span class="sxs-lookup"><span data-stu-id="df5c5-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="df5c5-109">Nurodykite vartotojo vardą vartotojo, kurį norite ištirti (vartotojo panaikinti elementus).</span><span class="sxs-lookup"><span data-stu-id="df5c5-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="df5c5-110">Šioje **veiklos** srityje, pasirinkite **panaikinti el. laiškai iš panaikintų elementų aplanką** ir **Moved laiškus į aplanką Panaikinta**.</span><span class="sxs-lookup"><span data-stu-id="df5c5-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="df5c5-111">Spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="df5c5-111">Click **Search**.</span></span>

<span data-ttu-id="df5c5-112">Rezultatų sąraše pasirinkite audito įrašas.</span><span class="sxs-lookup"><span data-stu-id="df5c5-112">In the results, select an audit record.</span></span> <span data-ttu-id="df5c5-113">Detalių išskleidžiamojo meniu spustelėkite **Daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="df5c5-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="df5c5-114">Papildomos informacijos apie panaikintas elementas (pvz., temos eilutė ir kai jis buvo panaikintas elemento vietą) nurodyta lauke **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="df5c5-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="df5c5-115">Ypatybę **ClientInfoString** parodys, jei naikinimą įvyko programoje "Outlook", "Outlook" žiniatinklyje (anksčiau žinomas kaip "Outlook Web App), arba kokio nors kito prietaiso.</span><span class="sxs-lookup"><span data-stu-id="df5c5-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="df5c5-116">Norėdami gauti daugiau informacijos, peržiūrėkite [renkant, kuris sukūrė el. pašto peradresavimo pašto dėžutės](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="df5c5-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="df5c5-117">**Pastaba**: jūs negalite gauti pašalinta naudojant funkciją audito žurnale.</span><span class="sxs-lookup"><span data-stu-id="df5c5-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="df5c5-118">Norėdami atkurti panaikintus laiškus programoje "Outlook" žiniatinklyje, peržiūrėkite [Atkurti panaikintus elementus Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="df5c5-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
