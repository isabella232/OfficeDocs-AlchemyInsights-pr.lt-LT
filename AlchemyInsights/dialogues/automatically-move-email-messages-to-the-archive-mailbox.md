---
title: Automatinis el. laiškų perkėlimas į archyvo pašto dėžutę
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527106"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="eb0aa-102">Automatinis el. laiškų perkėlimas į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="eb0aa-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="eb0aa-103">Štai kaip nustatyti strategiją, kad automatiškai perkeltumėte vartotojo senąjį laišką į archyvo pašto dėžutę:</span><span class="sxs-lookup"><span data-stu-id="eb0aa-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="eb0aa-104">Eikite į [**saugos & atitikties**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **duomenų valdymo**  >  **archyvą** , kad patvirtintumėte, jog vartotojui buvo įgalinta archyvo pašto dėžutė.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="eb0aa-105">Jei ne, spustelėkite **įjungti** ir **taip** lauke įspėjimas.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="eb0aa-106">Eikite į " [**Exchange" administravimo centras > atitikties valdymo > saugojimo žymės**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="eb0aa-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="eb0aa-107">Pasirinkite + piktogramą, tada pasirinkite **automatiškai taikyti visai pašto dėžutei**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="eb0aa-108">Priskirkite pavadinimą saugojimo žymei ir pasirinkite **perkelti į archyvą**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="eb0aa-109">Saugojimo laikotarpiui nustatykite norimą laiką, pvz., 90 dienos.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="eb0aa-110">Spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-110">Click **Save**.</span></span>
5. <span data-ttu-id="eb0aa-111">Dabar sukurkite saugojimo strategiją: pasirinkite **išsaugojimo strategijas**, pasirinkite piktogramą, kad įtrauktumėte naują strategiją.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="eb0aa-112">Priskirkite pavadinimą saugojimo strategijai, tada spustelėkite ir slinkite, kad rastumėte ir įtrauktumėte ką tik sukurtą saugojimo žymę.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="eb0aa-113">Spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-113">Click **Save**.</span></span>
7. <span data-ttu-id="eb0aa-114">Galiausiai pritaikykite saugojimo strategiją vartotojo pašto dėžutei: vis dar "Exchange" administravimo centre eikite į **gavėjų**  >  **pašto dėžutės**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="eb0aa-115">Pasirinkite visus vartotojus, kuriems norite taikyti strategiją, tada pasirinkite **Redaguoti** (pieštuko piktogramą).</span><span class="sxs-lookup"><span data-stu-id="eb0aa-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="eb0aa-116">Dialogo lange spustelėkite **pašto dėžutės funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="eb0aa-117">Dalyje **saugojimo strategija** taikykite ką tik sukurtą strategiją > **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="eb0aa-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="eb0aa-118">Nurodymų, kaip taikyti strategiją visiems vartotojams, ieškokite [išsaugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="eb0aa-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
