---
title: "\"Outlook Desktop\" atšaukimas arba pakeitimas el. laiško"
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496119"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="e4601-102">"Outlook" el. laiško atšaukimas arba keitimas</span><span class="sxs-lookup"><span data-stu-id="e4601-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="e4601-103">Kaip administratorius, galite **priminti pranešimus vartotojų vardu naudojant PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="e4601-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="e4601-104">Negalite atšaukti pranešimų iš administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="e4601-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="e4601-105">Galite **atšaukti tik tuos pranešimus, kurie siunčiami jūsų organizacijos žmonėms**.</span><span class="sxs-lookup"><span data-stu-id="e4601-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e4601-106">Jei pranešimas buvo išsiųstas "Gmail" adresu, pavyzdžiui, jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="e4601-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="e4601-107">Galite **tik atšaukti pranešimus, išsiųstus iš "Outlook 2016" kompiuteryje**.</span><span class="sxs-lookup"><span data-stu-id="e4601-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="e4601-108">Jei naudotojas siunčia pranešimą naudodamas "Outlook for Mac" arba "Outlook" žiniatinklyje, jo atšaukti negalite.</span><span class="sxs-lookup"><span data-stu-id="e4601-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="e4601-109">Jei norite atšaukti arba pakeisti el. laišką:</span><span class="sxs-lookup"><span data-stu-id="e4601-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="e4601-110">Kairėje "Outlook" lango aplanko srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="e4601-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="e4601-111">Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.</span><span class="sxs-lookup"><span data-stu-id="e4601-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="e4601-112">Pasirinkite skirtuką **pranešimas** , tada pasirinkite **veiksmai** > **prisiminti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="e4601-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="e4601-113">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **panaikinkite Neskaitytas kopijas ir pakeiskite nauju pranešimu**, tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="e4601-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="e4601-114">Jei siunčiate pakaitinį pranešimą, parašykite pranešimą, tada pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="e4601-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="e4601-115">Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo nustatymų "Outlook".</span><span class="sxs-lookup"><span data-stu-id="e4601-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="e4601-116">Norėdami sužinoti apie atšaukimo veiksmus, skaitykite [šį straipsnį](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="e4601-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e4601-117">Ieškoti ir naikinti el. laiškus organizacijoje</span><span class="sxs-lookup"><span data-stu-id="e4601-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="e4601-118">Jei nesate visuotinis administratorius, jūsų abonementas turi būti pridėtas prie eDiscovery Manager vaidmens arba atitikties ieškos valdymo vaidmens ieškant pranešimų.</span><span class="sxs-lookup"><span data-stu-id="e4601-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="e4601-119">Norėdami panaikinti pranešimus, turėsite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens.</span><span class="sxs-lookup"><span data-stu-id="e4601-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="e4601-120">Šių vaidmenų teisės priskiriamos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="e4601-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="e4601-121">[Sukurkite turinio iešką](https://docs.microsoft.com/office365/securitycompliance/content-search) , kad rastumėte naikindami pranešimą.</span><span class="sxs-lookup"><span data-stu-id="e4601-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="e4601-122">[Prisijungti prie saugos ir atitikties centro "PowerShell"](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e4601-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="e4601-123">Jei naudojate kelių dalių autentifikavimą, peržiūrėkite [prisijungti prie "Office 365" saugos ir atitikties centro "PowerShell" naudodami kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="e4601-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>