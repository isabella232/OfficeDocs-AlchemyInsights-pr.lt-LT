---
title: Nustatyti išorinės pašto persiuntimo pašto dėžučių audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752011"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="a5d62-102">Nustatyti sukonfigūravus pašto dėžutės išorinio el. pašto peradresavimas</span><span class="sxs-lookup"><span data-stu-id="a5d62-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="a5d62-103">Kai vartotojas konfigūruoja išorės el. laiškų peradresavimas į pašto dėžutę, veiklos auditą kaip į **Set-Mailbox** cmdlet.</span><span class="sxs-lookup"><span data-stu-id="a5d62-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="a5d62-104">Jūs galite pamatyti veiklos audito žurnalo paieškos naudojimas – saugos & atitikties užtikrinimo centre.</span><span class="sxs-lookup"><span data-stu-id="a5d62-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="a5d62-105">Prisijunkite prie [Office 365 saugumo & atitikties užtikrinimo centre](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="a5d62-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="a5d62-106">Spustelėkite **paieškos ir tyrimas** ir pasirinkite **Audito žurnalo paieška**.</span><span class="sxs-lookup"><span data-stu-id="a5d62-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="a5d62-107">Pasirinkite datos intervalą laukuose **pradžios data** ir **pabaigos data** .</span><span class="sxs-lookup"><span data-stu-id="a5d62-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a5d62-108">Jums nereikia nurodyti vartotojo vardą.</span><span class="sxs-lookup"><span data-stu-id="a5d62-108">You don't need to specify a username.</span></span> <span data-ttu-id="a5d62-109">Patikrinkite, ar **veiklos** laukas yra nustatytas **Rodyti visą veiklą, rezultatus**.</span><span class="sxs-lookup"><span data-stu-id="a5d62-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="a5d62-110">Spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="a5d62-110">Click **Search**.</span></span>

<span data-ttu-id="a5d62-111">Rezultatuose spustelėkite **Filtruoti rezultatus** ir veiklos filtras lauke įveskite **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="a5d62-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="a5d62-112">Pasirinkite įrašą audito rezultatus.</span><span class="sxs-lookup"><span data-stu-id="a5d62-112">Select an audit record in the results.</span></span> <span data-ttu-id="a5d62-113">**Detalių** išskleidžiamojo meniu spustelėkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="a5d62-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="a5d62-114">Jūs turite žiūrėti į išsamią informaciją apie kiekvieno audito įrašas nustatyti, jeigu veikla yra susijusi su el. pašto persiuntimas.</span><span class="sxs-lookup"><span data-stu-id="a5d62-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="a5d62-115">**ObjectId**: pseudonimas vertės pašto dėžutę, kuri buvo modifikuota.</span><span class="sxs-lookup"><span data-stu-id="a5d62-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="a5d62-116">**Parametrai**: _ForwardingSmtpAddress_ rodo, tikslinių el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="a5d62-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="a5d62-117">**Vartotojo ID**: vartotojo, kuris sukonfigūruotas el. pašto peradresavimas **ObjectId** srities pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="a5d62-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="a5d62-118">Norėdami gauti daugiau informacijos, peržiūrėkite [renkant, kuris sukūrė el. pašto peradresavimo pašto dėžutės](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a5d62-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
