---
title: Laiško atšaukimas arba pakeitimas
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353514"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="3289f-102">Laiško atšaukimas arba pakeitimas "Microsoft 365"</span><span class="sxs-lookup"><span data-stu-id="3289f-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="3289f-103">Galite **atšaukti tik tuos, kurie siunčiami į jūsų organizacijos žmones**.</span><span class="sxs-lookup"><span data-stu-id="3289f-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="3289f-104">Pavyzdžiui, jei laiškas buvo nusiųstas į "Gmail" adresą, jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="3289f-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="3289f-105">**Iš "Outlook" kompiuteriui siunčiamų žinučių galite atšaukti tik**.</span><span class="sxs-lookup"><span data-stu-id="3289f-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="3289f-106">Jei vartotojas siunčia laišką naudodamas "Outlook for Mac" arba internetinę "Outlook", jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="3289f-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="3289f-107">Kaip nuomotojo administratorius galite **Atšaukti vartotojų vardu esančius laiškus naudodami "PowerShell"** (daugiau informacijos rasite: [el. laiškų ieška ir naikinimas](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="3289f-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="3289f-108">Negalite atšaukti laiško administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="3289f-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="3289f-109">Norėdami gauti daugiau informacijos, slinkite žemyn iki "ieškoti ir naikinti el. laiškus organizacijoje".</span><span class="sxs-lookup"><span data-stu-id="3289f-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="3289f-110">**Atsiųsto el. laiško atšaukimas arba pakeitimas**</span><span class="sxs-lookup"><span data-stu-id="3289f-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="3289f-111">Programos "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="3289f-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="3289f-112">Atidarykite laišką, kurį norite atšaukti.</span><span class="sxs-lookup"><span data-stu-id="3289f-112">Open the message that you want to recall.</span></span> <span data-ttu-id="3289f-113">Norėdami atidaryti laišką, turite jį dukart spustelėti.</span><span class="sxs-lookup"><span data-stu-id="3289f-113">You must double-click to open the message.</span></span> <span data-ttu-id="3289f-114">Pažymėdami pranešimą, kad jis būtų rodomas skaitymo srityje, negalėsite atšaukti pranešimo.</span><span class="sxs-lookup"><span data-stu-id="3289f-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="3289f-115">Skirtuke laiškas pasirinkite **veiksmus**  >  **atšaukti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="3289f-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="3289f-116">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti Neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="3289f-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="3289f-117">Jei siunčiate pakaitinį pranešimą, parašykite pranešimą, tada pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="3289f-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="3289f-118">Laiško atšaukimo sėkmė arba gedimas priklauso nuo gavėjų parametrų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="3289f-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="3289f-119">Jei reikia daugiau informacijos, įskaitant tai, kaip patikrinti atšaukimą, žr. [pranešimo atšaukimas arba pakeitimas, kurį nusiuntėte](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="3289f-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="3289f-120">Jei norite **_Ieškoti ir naikinti el. laiškus organizacijoje_**, paprasčiausia, jei esate visuotinis administratorius. Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į "e" aptikimo tvarkytuvo vaidmenų grupę arba atitikties ieškos valdymo vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="3289f-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="3289f-121">Norėdami panaikinti laišką, turite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens.</span><span class="sxs-lookup"><span data-stu-id="3289f-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="3289f-122">Šių vaidmenų teisės priskirtos [saugos & atitikties centre](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="3289f-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="3289f-123">[Sukurkite turinio iešką](https://docs.microsoft.com/microsoft-365/compliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.</span><span class="sxs-lookup"><span data-stu-id="3289f-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="3289f-124">[Prisijunkite prie saugos & atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)".</span><span class="sxs-lookup"><span data-stu-id="3289f-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="3289f-125">Jei naudojate MFA (kelių dalių autentifikavimą), žiūrėkite [prisijungti prie "Microsoft 365" saugos & atitikties centro "PowerShell", naudodami kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3289f-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
