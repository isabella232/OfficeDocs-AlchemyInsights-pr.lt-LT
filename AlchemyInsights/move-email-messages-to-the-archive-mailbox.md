---
title: El. laiškų perkėlimas į archyvo pašto dėžutę
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522779"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="4f49d-102">El. laiško perkėlimas į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="4f49d-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="4f49d-103">Jei norite, kad mes vykdome automatinius patikrinimus dėl toliau nurodytų nustatymų, pasirinkite mygtuką "Atgal" < -- šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų perkeliant el. laišką į savo archyvo pašto dėžutę, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="4f49d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="4f49d-104">Patvirtinkite, kad **įgalinta archyvo pašto dėžutė.**</span><span class="sxs-lookup"><span data-stu-id="4f49d-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="4f49d-105">Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4f49d-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="4f49d-106">Norint automatiškai archyvuoti laiškus į archyvo pašto dėžutę, saugojimo žymė su veiksmu **Perkelti į archyvą** turi būti nustatyta **kaip automatiškai taikoma visai pašto dėžutei (numatytoji) žymei**.</span><span class="sxs-lookup"><span data-stu-id="4f49d-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="4f49d-107">Norėdami sukurti žymę, atlikite čia nurodytus veiksmus: [Archyvuoti numatytąją žymą](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="4f49d-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="4f49d-108">Tada pridėkite **žymę Archyvuoti** prie saugojimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="4f49d-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="4f49d-109">"Exchange" administravimo centre pasirinkite **Saugojimo strategijos** > į strategiją > **Įrašyti** **įtrauktumėte žymę Perkelti į archyvą** .</span><span class="sxs-lookup"><span data-stu-id="4f49d-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="4f49d-110">Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="4f49d-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="4f49d-111">Ta pati strategija bus taikoma ir **pirminio,** ir **archyvo** pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="4f49d-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="4f49d-112">Gali prireikti priversti valdomojo aplanko asistentas (DTS) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="4f49d-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="4f49d-113">Vykdykite šią komandą, kai [prijungtas prie EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) paleisti valdomos aplanko asistentas konkrečios pašto dėžutės:</span><span class="sxs-lookup"><span data-stu-id="4f49d-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="4f49d-114">Start-ManagedFolderAssistant -tapatybės<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="4f49d-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="4f49d-115">Daugiau informacijos apie archyvo strategijos nustatymą [ieškokite Pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="4f49d-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  