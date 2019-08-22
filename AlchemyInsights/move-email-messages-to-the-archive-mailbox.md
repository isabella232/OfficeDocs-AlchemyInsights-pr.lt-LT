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
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549011"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="4476f-102">Perkelti laišką į archyvo pašto dėžutę</span><span class="sxs-lookup"><span data-stu-id="4476f-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="4476f-103">Patvirtinkite, kad **archyvo pašto dėžutės** įgalintas.</span><span class="sxs-lookup"><span data-stu-id="4476f-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="4476f-104">Jei ne, atlikite veiksmus [šiame](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) straipsnyje, kad archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4476f-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="4476f-105">Jei norite archyvuoti pranešimus automatiškai į archyvo pašto dėžutę, saugojimo žymę **perkelti į archyvą** veikla turi būti nustatytas kaip **automatiškai taikomas visą dėžutę (numatytoji) žymę**.</span><span class="sxs-lookup"><span data-stu-id="4476f-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="4476f-106">Atlikite veiksmus čia sukurti žymę: [Archyvas numatytoji žymė](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="4476f-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>

3. <span data-ttu-id="4476f-107">Toliau, pridėkite **Archyvas** žymę su saugojimo strategija.</span><span class="sxs-lookup"><span data-stu-id="4476f-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="4476f-108">Exchange administravimo centrą, pasirinkite **Saugojimo strategijos** > pridėti **perkelti į archyvo žymių** **įrašyti**politikos >.</span><span class="sxs-lookup"><span data-stu-id="4476f-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="4476f-109">Dabar [priskirti saugojimo strategija](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) į konkrečius vartotojo pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="4476f-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="4476f-110">Ta pačia sutartimi taikysite į **pirminį** ir **archyvo** pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4476f-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="4476f-111">Reikia priversti valdomos aplanko asistentas (URM) vykdyti ir taikyti naujus parametrus vartotojo pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="4476f-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="4476f-112">Vykdykite šią komandą kol [prijungtas prie EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas:</span><span class="sxs-lookup"><span data-stu-id="4476f-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="4476f-113">Pradžia-ManagedFolderAssistant-tapatybė<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="4476f-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="4476f-114">Daugiau informacijos apie archyvavimo strategijos nustatymą, žiūrėkite [nustatyti archyvavimo ir naikinimo politiką pašto dėžučių](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="4476f-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  