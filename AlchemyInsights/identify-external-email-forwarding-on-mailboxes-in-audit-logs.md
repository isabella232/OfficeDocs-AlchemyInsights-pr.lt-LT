---
title: Nustatyti išorinį el. pašto peradresavimą pašto dėžutėse audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716468"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="379b8-102">Nustatyti, kada išorinių el. laiškų peradresavimas sukonfigūruotas pašto dėžutėse</span><span class="sxs-lookup"><span data-stu-id="379b8-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="379b8-103">Kai "Microsoft 365" vartotojas konfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla audituojama kaip **Set-Mailbox** cmdlet dalis.</span><span class="sxs-lookup"><span data-stu-id="379b8-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="379b8-104">Veiklą galite peržiūrėti naudodami audito žurnalo iešką saugos & atitikties centre.</span><span class="sxs-lookup"><span data-stu-id="379b8-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="379b8-105">Prisijunkite prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="379b8-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="379b8-106">Eikite į **ieškos** > **tikrinimo žurnalo ieškos** puslapį.</span><span class="sxs-lookup"><span data-stu-id="379b8-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="379b8-107">Laukuose **Pradžios data** ir **Pabaigos data** pasirinkite dienų seką.</span><span class="sxs-lookup"><span data-stu-id="379b8-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="379b8-108">Nebūtina nurodyti naudotojo vardo.</span><span class="sxs-lookup"><span data-stu-id="379b8-108">You don't need to specify a username.</span></span> <span data-ttu-id="379b8-109">Patikrinkite, ar laukas **Veiklos** nustatyta rodyti **visų veiklų rezultatus.**</span><span class="sxs-lookup"><span data-stu-id="379b8-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="379b8-110">Spustelėkite **Ieškoti**.</span><span class="sxs-lookup"><span data-stu-id="379b8-110">Click **Search**.</span></span>

<span data-ttu-id="379b8-111">Rezultatuose spustelėkite **Filtruoti rezultatus** ir veiklos filtro lauke įveskite **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="379b8-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="379b8-112">Rezultatuose pasirinkite audito įrašą.</span><span class="sxs-lookup"><span data-stu-id="379b8-112">Select an audit record in the results.</span></span> <span data-ttu-id="379b8-113">Iškeliamame pranešime **Išsami informacija** spustelėkite **Daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="379b8-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="379b8-114">Turite peržiūrėti kiekvieno audito įrašo informaciją, kad nustatytumėte, ar veikla susijusi su el. pašto peradresavimu.</span><span class="sxs-lookup"><span data-stu-id="379b8-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="379b8-115">**ObjectId**: Modifikuotos pašto dėžutės pseudonimo reikšmė.</span><span class="sxs-lookup"><span data-stu-id="379b8-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="379b8-116">**Parametrai**: _ForwardingSmtpAddress_ nurodo paskirties el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="379b8-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="379b8-117">**UserId**: Vartotojas, kuris sukonfigūravo el. pašto peradresavimą pašto dėžutės **objectid** lauke.</span><span class="sxs-lookup"><span data-stu-id="379b8-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="379b8-118">Daugiau informacijos [ieškokite Nustatymas, kas nustato pašto dėžutės el. pašto peradresavimą](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="379b8-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
