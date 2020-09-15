---
title: "\"Outlook\" kompiuterio atšaukimas arba pranešimo apie laišką keitimas"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663998"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="968e7-102">"Outlook" el. laiško atšaukimas arba pakeitimas</span><span class="sxs-lookup"><span data-stu-id="968e7-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="968e7-103">Kaip administratorius galite **Atšaukti vartotojų vardu naudodami "PowerShell"**.</span><span class="sxs-lookup"><span data-stu-id="968e7-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="968e7-104">Negalite atšaukti laiško administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="968e7-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="968e7-105">Galite **atšaukti tik tuos, kurie siunčiami į jūsų organizacijos žmones**.</span><span class="sxs-lookup"><span data-stu-id="968e7-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="968e7-106">Jei laiškas buvo išsiųstas į "Gmail" adresą, pvz., jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="968e7-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="968e7-107">Galite **tik atšaukti iš "Outlook 2016" išsiųstus "PC"**.</span><span class="sxs-lookup"><span data-stu-id="968e7-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="968e7-108">Jei vartotojas siunčia laišką naudodamas "Outlook for Mac" arba internetinę "Outlook", jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="968e7-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="968e7-109">Norėdami atšaukti arba pakeisti el. laišką:</span><span class="sxs-lookup"><span data-stu-id="968e7-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="968e7-110">Programos "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="968e7-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="968e7-111">Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.</span><span class="sxs-lookup"><span data-stu-id="968e7-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="968e7-112">Pasirinkite skirtuką **pranešimas** , tada pasirinkite **veiksmai**  >  **atšaukti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="968e7-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="968e7-113">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti Neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="968e7-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="968e7-114">Jei siunčiate pakaitinį pranešimą, parašykite laišką ir pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="968e7-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="968e7-115">Laiško atšaukimo sėkmė arba gedimas priklauso nuo gavėjo parametrų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="968e7-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="968e7-116">Norėdami patikrinti, ar yra atšaukimo veiksmų, peržiūrėkite [šį straipsnį](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="968e7-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="968e7-117">Savo organizacijos el. laiškų ieška ir naikinimas</span><span class="sxs-lookup"><span data-stu-id="968e7-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="968e7-118">Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į "e. Discovery Manager" vaidmenį arba atitikties ieškos valdymą, kad būtų ieškoma žinučių.</span><span class="sxs-lookup"><span data-stu-id="968e7-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="968e7-119">Norėdami panaikinti laišką, turite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens.</span><span class="sxs-lookup"><span data-stu-id="968e7-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="968e7-120">Šių vaidmenų teisės priskirtos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="968e7-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="968e7-121">[Sukurkite turinio iešką](https://docs.microsoft.com/microsoft-365/compliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.</span><span class="sxs-lookup"><span data-stu-id="968e7-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="968e7-122">[Prisijunkite prie saugos ir atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)".</span><span class="sxs-lookup"><span data-stu-id="968e7-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="968e7-123">Jei naudojate kelių dalių autentifikavimą, ieškokite [prisijungimas prie "Microsoft" 365 saugos ir atitikties centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="968e7-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>