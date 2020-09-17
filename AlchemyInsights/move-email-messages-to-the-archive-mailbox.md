---
title: Laiškų perkėlimas į archyvo pašto dėžutę
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799788"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="afe2e-102">Perkelti laišką į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="afe2e-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="afe2e-103">Jei norite, kad būtų atlikti automatizuoti toliau nurodytų parametrų tikrinimai, pasirinkite mygtuką atgal <--šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų perkeliant laiškus į archyvo pašto dėžutę, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="afe2e-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="afe2e-104">Patikrinkite, ar įgalintas **archyvo pašto dėžutė** .</span><span class="sxs-lookup"><span data-stu-id="afe2e-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="afe2e-105">Jei ne, atlikite [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) nurodytus veiksmus, kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="afe2e-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="afe2e-106">Kad laiškai automatiškai būtų archyvuojami į archyvo pašto dėžutę, saugojimo žymė su veiksmu **perkelti į archyvą** turi būti nustatyta **automatiškai pritaikyta visai pašto dėžutei (numatytoji)**.</span><span class="sxs-lookup"><span data-stu-id="afe2e-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="afe2e-107">Atlikite toliau nurodytus veiksmus, kad sukurtumėte žymę: [archyvuoti numatytąjį žymę](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="afe2e-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="afe2e-108">Tada įtraukite **archyvo** žymę į saugojimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="afe2e-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="afe2e-109">"Exchange" administravimo centre pasirinkite **saugojimo strategijos** > įtraukite **perkėlimo į archyvą žymę** į strategiją > **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="afe2e-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="afe2e-110">Dabar [priskirkite saugojimo strategiją](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrečiam vartotojo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="afe2e-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="afe2e-111">Ta pati strategija bus taikoma ir **pirminės** ir **archyvo** pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="afe2e-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="afe2e-112">Gali reikėti priverstinai vykdyti valdomojo aplanko asistentą (MFA) ir taikyti naujus parametrus vartotojo pašto dėžutei.</span><span class="sxs-lookup"><span data-stu-id="afe2e-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="afe2e-113">Norėdami paleisti konkrečios pašto dėžutės valdomojo aplanko asistentą, būdami [prisijungę prie "EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) " vykdykite šią komandą:</span><span class="sxs-lookup"><span data-stu-id="afe2e-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="afe2e-114">Start – ManagedFolderAssistant – tapatybė <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="afe2e-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="afe2e-115">Daugiau informacijos apie archyvavimo strategijos nustatymą rasite [pašto dėžučių archyvavimo ir naikinimo strategijos nustatymas](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="afe2e-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  