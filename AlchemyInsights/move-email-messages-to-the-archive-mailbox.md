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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713654"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5a6f8-102">El. pašto perkėlimas į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="5a6f8-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="5a6f8-103">Patvirtinkite, kad **įgalinta archyvo pašto dėžutė.**</span><span class="sxs-lookup"><span data-stu-id="5a6f8-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5a6f8-104">Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5a6f8-105">Norint automatiškai archyvuoti pranešimus į archyvo pašto dėžutę, saugojimo žyma su veiksmu **Perkelti į archyvą** turi būti nustatyta taip, kad automatiškai **būtų taikoma visai pašto dėžutei (numatytoji) žymai**.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5a6f8-106">Norėdami sukurti žymę, atlikite čia nurodytus veiksmus: [Archyvo numatytoji žymė](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5a6f8-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5a6f8-107">Tada įtraukite **archyvo** žymę į saugojimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5a6f8-108">"Exchange" administravimo centre pasirinkite **Saugojimo strategijos** > įtrauktumėte **žymę Perkelti į archyvą** į strategijos > **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5a6f8-109">Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5a6f8-110">Ta pati strategija bus taikoma ir **pirminio,** ir **archyvo** pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5a6f8-111">Gali tekti priversti valdomojo aplanko asistentas (DTS) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="5a6f8-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5a6f8-112">Norėdami paleisti konkrečios pašto dėžutės valdomos aplanko asistentą, [vykdykite](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) šią komandą:</span><span class="sxs-lookup"><span data-stu-id="5a6f8-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5a6f8-113">Start-ManagedFolderAssistant -tapatybės<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5a6f8-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5a6f8-114">Daugiau informacijos apie archyvo strategijos nustatymą ieškokite [Pašto dėžučių archyvo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5a6f8-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  