---
title: Archyvo pašto dėžutės įgalinimas
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811713"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="4483e-102">Archyvo pašto dėžutės įgalinimas</span><span class="sxs-lookup"><span data-stu-id="4483e-102">Enable an archive mailbox</span></span>

<span data-ttu-id="4483e-103">Jei norite, kad būtų galima atlikti automatinius patikrinimus, kad būtų galima sukonfigūruoti archyvo pašto dėžutę, pasirinkite grįžimo mygtuką < – šio puslapio viršuje, tada įveskite paskyros el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="4483e-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="4483e-104">"Microsoft 365" archyvo pašto dėžutės (taip pat vadinamos *internetiniais archyvais* arba *archyvuose vietoje*) teikia vartotojams papildomą elektroninio pašto saugyklą.</span><span class="sxs-lookup"><span data-stu-id="4483e-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="4483e-105">Vartotojai gali perkelti arba kopijuoti elementus į archyvo pašto dėžutę, o administratoriai gali sukurti archyvavimo strategiją, kuri automatiškai perkelia elementus į archyvo pašto dėžutes.</span><span class="sxs-lookup"><span data-stu-id="4483e-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="4483e-106">Štai kaip sukurti archyvo pašto dėžutę:</span><span class="sxs-lookup"><span data-stu-id="4483e-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="4483e-107">Eiti į [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="4483e-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="4483e-108">Prisijunkite prie "Microsoft 365" naudodami savo administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="4483e-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="4483e-109">Saugos &amp; atitikties centro kairiojoje srityje pasirinkite **informacijos valdymo** \> **Archyvas**.</span><span class="sxs-lookup"><span data-stu-id="4483e-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="4483e-110">Pasirinkite vartotoją, kurio archyvo pašto dėžutę norite įgalinti.</span><span class="sxs-lookup"><span data-stu-id="4483e-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="4483e-111">Dešinėje esančioje išsamios informacijos srityje spustelėkite **įgalinti** , tada įspėjimo pranešime spustelėkite **taip** , kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4483e-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="4483e-112">Be to, galite masiškai įgalinti archyvo pašto dėžutes pasirinkdami kelis vartotojus (naudodami klavišus **SHIFT** arba **Ctrl** ) ir spustelėkite **įgalinti** išsamios informacijos srityje.</span><span class="sxs-lookup"><span data-stu-id="4483e-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="4483e-113">Bendrinamos pašto dėžutės</span><span class="sxs-lookup"><span data-stu-id="4483e-113">Shared mailboxes</span></span>

<span data-ttu-id="4483e-114">Norint įgalinti bendrinamos pašto dėžutės archyvą, būtina turėti "Exchange Online" 2 plano licenciją arba "Exchange Online" 1 plano licenciją su "Exchange Online" archyvavimo licencija.</span><span class="sxs-lookup"><span data-stu-id="4483e-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="4483e-115">Norėdami įgalinti bendrinamos pašto dėžutės archyvą:</span><span class="sxs-lookup"><span data-stu-id="4483e-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="4483e-116">Eikite į " [Exchange" administravimo centrą](https://outlook.office365.com/ecp) ir prisijunkite naudodami savo administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="4483e-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="4483e-117">Eikite į **Recipients**  >  **bendrinamus**gavėjus.</span><span class="sxs-lookup"><span data-stu-id="4483e-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="4483e-118">Pasirinkite bendrinamą pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4483e-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="4483e-119">Dešinėje esančioje išsamios informacijos srityje, dalyje **vietos Archyvas**, spustelėkite **įgalinti**, tada spustelėkite **taip** , kad įgalintumėte archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="4483e-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="4483e-120">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="4483e-120">For more information, see:</span></span>
  
- [<span data-ttu-id="4483e-121">Archyvo pašto dėžučių įgalinimas</span><span class="sxs-lookup"><span data-stu-id="4483e-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="4483e-122">Archyvavimo ir naikinimo strategijos nustatymas</span><span class="sxs-lookup"><span data-stu-id="4483e-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
