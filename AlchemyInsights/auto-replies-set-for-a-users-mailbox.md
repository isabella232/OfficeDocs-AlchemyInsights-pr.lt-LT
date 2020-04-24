---
title: Automatinių atsakymų nustatymas pašto dėžutei
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788890"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="b2df3-102">Automatinių atsakymų nustatymas vartotojo pašto dėžutei</span><span class="sxs-lookup"><span data-stu-id="b2df3-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="b2df3-103">**1 būdas**</span><span class="sxs-lookup"><span data-stu-id="b2df3-103">**Method 1**</span></span>

1. <span data-ttu-id="b2df3-104">Prisijunkite prie „Microsoft 365“ portalo.</span><span class="sxs-lookup"><span data-stu-id="b2df3-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="b2df3-105">Eikite į **Vartotojai > Aktyvūs vartotojai** (arba **Grupės > Bendrinamos pašto dėžutės**, jei nustatote bendrai naudojamai pašto dėžutei).</span><span class="sxs-lookup"><span data-stu-id="b2df3-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="b2df3-106">Pasirinkite vartotoją, kuris turi „Microsoft Exchange“ pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="b2df3-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="b2df3-107">Dešiniajame išskleidžiamajame meniu eikite į **Pašto parametrai > Automatiniai atsakymai** (jei tai bendrinama pašto dėžutė, išskleidžiamajame meniu spustelėkite **Automatiniai atsakymai**).</span><span class="sxs-lookup"><span data-stu-id="b2df3-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="b2df3-108">**2 būdas**</span><span class="sxs-lookup"><span data-stu-id="b2df3-108">**Method 2**</span></span>

1. <span data-ttu-id="b2df3-109">Prisijunkite prie „Microsoft 365“ administravimo portalo naudodami administratoriaus kredencialus.</span><span class="sxs-lookup"><span data-stu-id="b2df3-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="b2df3-110">Išplėskite **Administravimo centrai**, tada spustelėkite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b2df3-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="b2df3-111">Viršutiniame dešiniajame kampe spustelėkite paveikslėlį, spustelėkite **Kitas vartotojas**, tada pasirinkite vartotojo pašto dėžutę, kurią norite keisti.</span><span class="sxs-lookup"><span data-stu-id="b2df3-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="b2df3-112">Kairiojoje pusėje pasirinkite **Parinktys**, spustelėkite **Tvarkyti el. paštą**, tada spustelėkite **Automatiniai atsakymai.**</span><span class="sxs-lookup"><span data-stu-id="b2df3-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="b2df3-113">**3 būdas**</span><span class="sxs-lookup"><span data-stu-id="b2df3-113">**Method 3**</span></span>

<span data-ttu-id="b2df3-114">„Exchange Online PowerShell“ vykdykite tolesnę cmdlet:</span><span class="sxs-lookup"><span data-stu-id="b2df3-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b2df3-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b2df3-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="b2df3-116">Daugiau informacijos apie šią cmdlet žr. [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="b2df3-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
