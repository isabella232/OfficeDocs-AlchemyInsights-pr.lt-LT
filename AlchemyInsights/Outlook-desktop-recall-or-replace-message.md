---
title: "\"Outlook\" darbalaukio atšaukimas arba el. laiško keitimas"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502327"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="dfbbb-102">"Outlook" el. laiško atšaukimas arba keitimas</span><span class="sxs-lookup"><span data-stu-id="dfbbb-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="dfbbb-103">Kaip administratorius, galite **atšaukti pranešimus vartotojų vardu naudodami "PowerShell".**</span><span class="sxs-lookup"><span data-stu-id="dfbbb-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="dfbbb-104">Negalite atšaukti pranešimų iš administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="dfbbb-105">Galite **atšaukti tik tuos pranešimus, kurie siunčiami jūsų organizacijos žmonėms**.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="dfbbb-106">Pavyzdžiui, jei pranešimas buvo išsiųstas "Gmail" adresu, jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="dfbbb-107">Galite **atšaukti tik pranešimus, išsiųstus iš "Outlook 2016" kompiuteryje**.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="dfbbb-108">Jei vartotojas siunčia pranešimą naudodamas "Outlook for Mac" arba "Outlook" žiniatinklyje, jo atšaukti negalite.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="dfbbb-109">Norėdami atšaukti arba pakeisti el. laišką:</span><span class="sxs-lookup"><span data-stu-id="dfbbb-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="dfbbb-110">"Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="dfbbb-111">Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="dfbbb-112">Pasirinkite skirtuką **Pranešimas,** tada pasirinkite **Veiksmai**  >  **Atšaukti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="dfbbb-113">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="dfbbb-114">Jei siunčiate pakaitinį pranešimą, sukurkite pranešimą, tada pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="dfbbb-115">Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo parametrų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="dfbbb-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="dfbbb-116">Veiksmus, kuriuos reikia patikrinti atšaukimo, ieškokite [šiame straipsnyje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="dfbbb-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="dfbbb-117">El. laiškų ieška ir naikinimas organizacijoje</span><span class="sxs-lookup"><span data-stu-id="dfbbb-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="dfbbb-118">Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į el. duomenų aptikimo tvarkytuvo vaidmenį arba atitikties ieškos valdymo vaidmenį, kad būtų ieškoma pranešimų.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="dfbbb-119">Norėdami panaikinti pranešimus, turėsite prisijungti prie vaidmenų grupės Organizacijos valdymas arba ieškos ir valymo valdymo vaidmens.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="dfbbb-120">Šių vaidmenų teisės priskiriamos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="dfbbb-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="dfbbb-121">[Sukurkite turinio iešką,](https://docs.microsoft.com/microsoft-365/compliance/content-search) kad rastumėte naikintiną pranešimą.</span><span class="sxs-lookup"><span data-stu-id="dfbbb-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="dfbbb-122">[Prisijunkite prie saugos ir atitikties centro "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="dfbbb-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="dfbbb-123">Jei naudojate kelių dalių autentifikavimą, [žr.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="dfbbb-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>