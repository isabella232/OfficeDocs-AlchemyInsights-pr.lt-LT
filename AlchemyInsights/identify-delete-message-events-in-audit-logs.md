---
title: Pranešimų naikinimo įvykių atpažinimas audito žurnaluose
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696521"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="c5966-102">Panaikintų el. laiškų audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="c5966-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="c5966-103">Nuo sausio 2019 d. "Microsoft" pagal numatytuosius numatytuosius pašto dėžučių audito žurnalus įjunkite.</span><span class="sxs-lookup"><span data-stu-id="c5966-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="c5966-104">Kitu atveju Norėdami peržiūrėti konkretaus vartotojo panaikintų pranešimų įvykius, turite rankiniu būdu įgalinti tikrinimo veiksmų naikinimo veiksmus.</span><span class="sxs-lookup"><span data-stu-id="c5966-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="c5966-105">Jei pašto dėžutės audito registravimas jau įgalintas jūsų organizacijai arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="c5966-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="c5966-106">Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c5966-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c5966-107">Spustelėkite **ieška ir tyrimas** ir pasirinkite **audito žurnalų ieška**.</span><span class="sxs-lookup"><span data-stu-id="c5966-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c5966-108">Laukuose **pradžios data** ir **pabaigos data** pasirinkite datų intervalą.</span><span class="sxs-lookup"><span data-stu-id="c5966-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c5966-109">Nurodo vartotojo, kurį norite analizuoti, vartotojo vardą (vartotojas, kuris panaikino elementus).</span><span class="sxs-lookup"><span data-stu-id="c5966-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="c5966-110">Lauke **veikla** pasirinkite **pašalinti laiškai iš panaikintų elementų aplanko** ir **perkelti laiškus į aplanką Panaikinta**.</span><span class="sxs-lookup"><span data-stu-id="c5966-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="c5966-111">Spustelėkite **ieška**.</span><span class="sxs-lookup"><span data-stu-id="c5966-111">Click **Search**.</span></span>

<span data-ttu-id="c5966-112">Rezultatuose pasirinkite audito įrašą.</span><span class="sxs-lookup"><span data-stu-id="c5966-112">In the results, select an audit record.</span></span> <span data-ttu-id="c5966-113">Išsamios informacijos išskridimas spustelėkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="c5966-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c5966-114">Papildoma informacija apie panaikintą elementą (pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas) rodoma lauke **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="c5966-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="c5966-115">Ypatybė **Clientinfostring** bus rodoma, jei jis buvo panaikintas programoje "Outlook", "Outlook" žiniatinklyje (anksčiau – "Outlook Web App") arba bet kurį kitą įrenginį.</span><span class="sxs-lookup"><span data-stu-id="c5966-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="c5966-116">Daugiau informacijos ieškokite kaip [nustatyti, kas nustato pašto dėžutės pašto peradresavimą](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="c5966-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="c5966-117">**Pastaba**: panaikintų elementų atkurti negalima naudojant audito žurnalų funkciją.</span><span class="sxs-lookup"><span data-stu-id="c5966-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="c5966-118">Norėdami atkurti panaikintus laiškus internetinėje "Outlook", peržiūrėkite [panaikintų elementų atkūrimas "Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)".</span><span class="sxs-lookup"><span data-stu-id="c5966-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
