---
title: Nustatyti naikinimo pranešimų įvykius audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508996"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="a47ef-102">Panaikintų el. laiškų audito žurnalai</span><span class="sxs-lookup"><span data-stu-id="a47ef-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="a47ef-103">Nuo 2019 m. sausio , "Microsoft" įjungia pašto dėžutės audito registravimą pagal numatytuosius nustatymus.</span><span class="sxs-lookup"><span data-stu-id="a47ef-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="a47ef-104">Kitu atveju, jei norite peržiūrėti konkretaus vartotojo pranešimų naikinimo įvykius, turite rankiniu būdu įgalinti tikrinimo naikinimo veiksmus.</span><span class="sxs-lookup"><span data-stu-id="a47ef-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="a47ef-105">Jei pašto dėžučių audito registravimas jau įgalintas jūsų organizacijoje arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="a47ef-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="a47ef-106">Prisijunkite prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="a47ef-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="a47ef-107">Spustelėkite **Ieškoti ir tirti** ir pasirinkite Audito **žurnalo ieška**.</span><span class="sxs-lookup"><span data-stu-id="a47ef-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="a47ef-108">Laukuose **Pradžios data** ir **Pabaigos data** pasirinkite dienų seką.</span><span class="sxs-lookup"><span data-stu-id="a47ef-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a47ef-109">Nurodykite vartotojo, kurį norite ištirti, vartotojo vardą (vartotoją, kuris panaikino elementus).</span><span class="sxs-lookup"><span data-stu-id="a47ef-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="a47ef-110">Lauke **Veikla** pasirinkite **Panaikinti pranešimai iš aplanko Pašalinta** ir **Perkelti pranešimai į aplanką Pašalinta**.</span><span class="sxs-lookup"><span data-stu-id="a47ef-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="a47ef-111">Spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="a47ef-111">Click **Search**.</span></span>

<span data-ttu-id="a47ef-112">Rezultatuose pasirinkite audito įrašą.</span><span class="sxs-lookup"><span data-stu-id="a47ef-112">In the results, select an audit record.</span></span> <span data-ttu-id="a47ef-113">Išsamios informacijos iškeliamamejį meniu spustelėkite **Daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="a47ef-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="a47ef-114">Papildoma informacija apie panaikintą elementą (pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas) rodoma lauke **Susijusio Elementai.**</span><span class="sxs-lookup"><span data-stu-id="a47ef-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="a47ef-115">**Ypatybė ClientInfoString** bus rodoma, jei naikinimas įvyko programoje "Outlook", "Outlook" žiniatinklyje (anksčiau vadinta "Outlook Web App") ar bet kuriame kitame įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="a47ef-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="a47ef-116">Daugiau informacijos [ieškokite Nustatymas, kas nustato pašto dėžutės el. pašto peradresavimą](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="a47ef-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="a47ef-117">**Pastaba:** negalite nuskaityti panaikintų elementų naudodami audito žurnalo funkciją.</span><span class="sxs-lookup"><span data-stu-id="a47ef-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="a47ef-118">Norėdami nuskaityti panaikintus pranešimus internetinėje "Outlook", žiūrėkite [Panaikintų elementų atkūrimas "Outlook Web App".](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)</span><span class="sxs-lookup"><span data-stu-id="a47ef-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
