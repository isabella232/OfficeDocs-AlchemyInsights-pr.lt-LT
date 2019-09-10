---
title: Perkelti el. laiškus į archyvo pašto dėžutę
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822170"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="3ce1b-102">Perkelti el. paštą į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="3ce1b-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="3ce1b-103">Patvirtinkite, kad įgalinta **archyvo pašto dėžutė** .</span><span class="sxs-lookup"><span data-stu-id="3ce1b-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="3ce1b-104">Jei ne, naudokite [šiame straipsnyje](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="3ce1b-105">Norint automatiškai archyvuoti pranešimus į archyvo pašto dėžutę, saugojimo žymė su veiksmu **perkelti į archyvą** turi būti nustatyta **automatiškai taikoma visai pašto dėžutei (numatytoji) žymėje**.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="3ce1b-106">Norėdami sukurti žymę, pasinaudokite čia esančiais žingsniais: [archyvuokite numatytąją žymę](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="3ce1b-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="3ce1b-107">Tada pridėkite **archyvo** žymę prie saugojimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="3ce1b-108">"Exchange" administravimo centre pasirinkite **saugojimo strategijos** > įtraukite **perkelti į archyvą žymę** į strategiją > **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="3ce1b-109">Dabar [priskirti saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="3ce1b-110">Ta pati strategija bus taikoma ir **pirminei** , ir **archyvo** pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="3ce1b-111">Gali reikėti priversti valdomojo aplanko asistentą (MFP) paleisti ir taikyti naujus parametrus vartotojo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="3ce1b-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="3ce1b-112">Kai [prisijungėte prie "EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) " Norėdami paleisti konkrečios pašto dėžutės valdomojo aplanko asistentą, vykdykite šią komandą:</span><span class="sxs-lookup"><span data-stu-id="3ce1b-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="3ce1b-113">Start-ManagedFolderAssistant-tapatybė<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="3ce1b-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="3ce1b-114">Daugiau informacijos apie archyvavimo strategijos nustatymą ieškokite [pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="3ce1b-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  