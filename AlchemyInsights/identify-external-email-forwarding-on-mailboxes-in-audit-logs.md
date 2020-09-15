---
title: Išorinių laiškų peradresavimo pašto dėžutėse nustatymas audito žurnaluose
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696305"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="58cf0-102">Atpažinimas, kai išoriniai pašto peradresavimas yra sukonfigūruotas pašto dėžutėse</span><span class="sxs-lookup"><span data-stu-id="58cf0-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="58cf0-103">Kai "Microsoft 365" vartotojo konfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla tikrinama kaip **Set-Mailbox** cmdlet dalis.</span><span class="sxs-lookup"><span data-stu-id="58cf0-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="58cf0-104">Galite peržiūrėti veiklą naudodami audito žurnalų iešką saugos & atitikties centre.</span><span class="sxs-lookup"><span data-stu-id="58cf0-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="58cf0-105">Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="58cf0-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="58cf0-106">Eikite į puslapį **ieškos**  >  **audito žurnalų ieška** .</span><span class="sxs-lookup"><span data-stu-id="58cf0-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="58cf0-107">Laukuose **pradžios data** ir **pabaigos data** pasirinkite datų intervalą.</span><span class="sxs-lookup"><span data-stu-id="58cf0-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="58cf0-108">Jums nereikia įvesti vartotojo vardo.</span><span class="sxs-lookup"><span data-stu-id="58cf0-108">You don't need to specify a username.</span></span> <span data-ttu-id="58cf0-109">Patikrinkite, ar laukas **veikla** nustatytas **Rodyti visų veiklų rezultatus**.</span><span class="sxs-lookup"><span data-stu-id="58cf0-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="58cf0-110">Spustelėkite **ieška**.</span><span class="sxs-lookup"><span data-stu-id="58cf0-110">Click **Search**.</span></span>

<span data-ttu-id="58cf0-111">Rezultatuose spustelėkite **filtruoti rezultatus** ir įveskite **Set-Mailbox** lauke veiklos filtras.</span><span class="sxs-lookup"><span data-stu-id="58cf0-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="58cf0-112">Rezultatuose pasirinkite audito įrašą.</span><span class="sxs-lookup"><span data-stu-id="58cf0-112">Select an audit record in the results.</span></span> <span data-ttu-id="58cf0-113">**Išsamios informacijos** išskridimas spustelėkite **daugiau informacijos**.</span><span class="sxs-lookup"><span data-stu-id="58cf0-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="58cf0-114">Turite pažiūrėti kiekvieno audito įrašo išsamią informaciją, kad nustatytumėte, ar veikla susijusi su elektroninio pašto peradresavimu.</span><span class="sxs-lookup"><span data-stu-id="58cf0-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="58cf0-115">**ObjectId**: pakeistos pašto dėžutės pseudonimo reikšmė.</span><span class="sxs-lookup"><span data-stu-id="58cf0-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="58cf0-116">**Parametrai**: " _forwardingsmt paddress_ " nurodo tikslinį elektroninio pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="58cf0-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="58cf0-117">**UserID**: vartotojas, sukonfigūravęs pašto peradresavimo funkciją lauke **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="58cf0-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="58cf0-118">Daugiau informacijos ieškokite kaip [nustatyti, kas nustato pašto dėžutės pašto peradresavimą](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="58cf0-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
