---
title: Automatinių atsakymų nustatymas pašto dėžutei
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820942"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="ed214-102">Automatinių atsakymų nustatymas vartotojo pašto dėžutei</span><span class="sxs-lookup"><span data-stu-id="ed214-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="ed214-103">**1 būdas**</span><span class="sxs-lookup"><span data-stu-id="ed214-103">**Method 1**</span></span>

1. <span data-ttu-id="ed214-104">Prisijunkite prie „Microsoft 365“ portalo.</span><span class="sxs-lookup"><span data-stu-id="ed214-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="ed214-105">Eikite į **Vartotojai > Aktyvūs vartotojai** (arba **Grupės > Bendrinamos pašto dėžutės**, jei nustatote bendrai naudojamai pašto dėžutei).</span><span class="sxs-lookup"><span data-stu-id="ed214-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="ed214-106">Pasirinkite vartotoją, kuris turi „Microsoft Exchange“ pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="ed214-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="ed214-107">Dešiniajame išskleidžiamajame meniu eikite į **Pašto parametrai > Automatiniai atsakymai** (jei tai bendrinama pašto dėžutė, išskleidžiamajame meniu spustelėkite **Automatiniai atsakymai**).</span><span class="sxs-lookup"><span data-stu-id="ed214-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="ed214-108">**2 būdas**</span><span class="sxs-lookup"><span data-stu-id="ed214-108">**Method 2**</span></span>

1. <span data-ttu-id="ed214-109">Prisijunkite prie „Microsoft 365“ administravimo portalo naudodami administratoriaus kredencialus.</span><span class="sxs-lookup"><span data-stu-id="ed214-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="ed214-110">Išplėskite **Administravimo centrai**, tada spustelėkite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ed214-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="ed214-111">Viršutiniame dešiniajame kampe spustelėkite paveikslėlį, spustelėkite **Kitas vartotojas**, tada pasirinkite vartotojo pašto dėžutę, kurią norite keisti.</span><span class="sxs-lookup"><span data-stu-id="ed214-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="ed214-112">Kairiojoje pusėje pasirinkite **Parinktys**, spustelėkite **Tvarkyti el. paštą**, tada spustelėkite **Automatiniai atsakymai.**</span><span class="sxs-lookup"><span data-stu-id="ed214-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="ed214-113">**3 būdas**</span><span class="sxs-lookup"><span data-stu-id="ed214-113">**Method 3**</span></span>

<span data-ttu-id="ed214-114">„Exchange Online PowerShell“ vykdykite tolesnę cmdlet:</span><span class="sxs-lookup"><span data-stu-id="ed214-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="ed214-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="ed214-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="ed214-116">Daugiau informacijos apie šią cmdlet žr. [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="ed214-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
