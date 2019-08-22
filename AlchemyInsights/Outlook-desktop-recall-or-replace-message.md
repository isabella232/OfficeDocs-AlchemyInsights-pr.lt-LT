---
title: "\"Outlook\" darbalaukio atšaukti ar keisti el. paštu"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496119"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="084f8-102">Atšaukti arba pakeisti "Outlook" el. laiško</span><span class="sxs-lookup"><span data-stu-id="084f8-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="084f8-103">Kaip administratorius, galite **Atšaukti pranešimų vardu vartotojai naudodami "PowerShell"**.</span><span class="sxs-lookup"><span data-stu-id="084f8-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="084f8-104">Jūs negalite prisiminti pranešimus administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="084f8-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="084f8-105">Jūs galite **tik priminti pranešimus, kurie siunčiami jūsų organizacijos žmonės**.</span><span class="sxs-lookup"><span data-stu-id="084f8-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="084f8-106">Jei pranešimas buvo išsiųstas į "Gmail" adresą, pvz., jūs negalite prisiminti jį.</span><span class="sxs-lookup"><span data-stu-id="084f8-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="084f8-107">Jūs galite **tik prisiminti laiškus iš "Outlook" 2016 kompiuteryje**.</span><span class="sxs-lookup"><span data-stu-id="084f8-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="084f8-108">Jei vartotojo siunčia pranešimą naudodami "Outlook" skirtas "Mac" arba "Outlook" internete, negali prisiminti jį.</span><span class="sxs-lookup"><span data-stu-id="084f8-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="084f8-109">Atšaukti arba pakeisti el. paštu:</span><span class="sxs-lookup"><span data-stu-id="084f8-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="084f8-110">Aplanką "Outlook" lango kairėje srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="084f8-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="084f8-111">Dukart spustelėkite pranešimą, Norėdami priminti, kad jį atidarytumėte.</span><span class="sxs-lookup"><span data-stu-id="084f8-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="084f8-112">Pasirinkite **laiško** skirtuko ir pasirinkite **veiksmai** > **Atšaukti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="084f8-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="084f8-113">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Neskaitytas kopijas naikinti ir keisti nauju pranešimu**, ir pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="084f8-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="084f8-114">Jei siunčiate žinutę pakeitimo, parašyti žinutę ir pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="084f8-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="084f8-115">Sėkmę ar nesėkmę, pranešimo atšaukimas priklauso nuo gavėjo pašto parametrų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="084f8-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="084f8-116">Patikrinti atšaukti veiksmus, ieškokite [šiame straipsnyje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="084f8-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="084f8-117">Ieškoti ir panaikinti el. laiškus į jūsų organizacijos</span><span class="sxs-lookup"><span data-stu-id="084f8-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="084f8-118">Jei nesate visuotinio administravimo, jūsų paskyra įrašoma į eDiscovery vadovo vaidmuo arba atitikties paieškos valdymo vaidmuo ieškoti laiškų.</span><span class="sxs-lookup"><span data-stu-id="084f8-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="084f8-119">Norėdami ištrinti pranešimus, jums reikia prisijungti prie vaidmenų grupės organizacijos valdymas arba paieškos ir prapūtimo valdymo vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="084f8-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="084f8-120">Teises rolėms priskirti [saugos ir atitikties užtikrinimo centre](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="084f8-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="084f8-121">[Kurti turinio ieškoti](https://docs.microsoft.com/office365/securitycompliance/content-search) ir rasti žinutę ištrinti.</span><span class="sxs-lookup"><span data-stu-id="084f8-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="084f8-122">[Prisijungti prie saugos ir atitikties užtikrinimo centre "PowerShell"](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="084f8-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="084f8-123">Jei naudojate kelių dalių autentifikavimas, pamatyti [prisijungti prie "Office 365" sauga ir atitiktis centras "PowerShell" naudoja kelių dalių autentifikavimas](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="084f8-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>