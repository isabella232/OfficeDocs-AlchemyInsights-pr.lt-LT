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
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687518"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="53621-102">"Outlook" el. laiško atšaukimas arba keitimas</span><span class="sxs-lookup"><span data-stu-id="53621-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="53621-103">Kaip administratorius, galite **atšaukti pranešimus vartotojų vardu naudodami "PowerShell".**</span><span class="sxs-lookup"><span data-stu-id="53621-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="53621-104">Negalite atšaukti pranešimų iš administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="53621-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="53621-105">Galite **atšaukti tik tuos pranešimus, kurie siunčiami jūsų organizacijos žmonėms**.</span><span class="sxs-lookup"><span data-stu-id="53621-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="53621-106">Pavyzdžiui, jei pranešimas buvo išsiųstas "Gmail" adresu, jo atšaukti negalėsite.</span><span class="sxs-lookup"><span data-stu-id="53621-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="53621-107">Galite **atšaukti tik pranešimus, išsiųstus iš "Outlook 2016" kompiuteryje**.</span><span class="sxs-lookup"><span data-stu-id="53621-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="53621-108">Jei vartotojas siunčia pranešimą naudodamas "Outlook for Mac" arba "Outlook" žiniatinklyje, jo atšaukti negalite.</span><span class="sxs-lookup"><span data-stu-id="53621-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="53621-109">Norėdami atšaukti arba pakeisti el. laišką:</span><span class="sxs-lookup"><span data-stu-id="53621-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="53621-110">"Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.</span><span class="sxs-lookup"><span data-stu-id="53621-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="53621-111">Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.</span><span class="sxs-lookup"><span data-stu-id="53621-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="53621-112">Pasirinkite skirtuką **Pranešimas,** tada pasirinkite **Veiksmai** > **Atšaukti šį pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="53621-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="53621-113">Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="53621-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="53621-114">Jei siunčiate pakaitinį pranešimą, sukurkite pranešimą, tada pasirinkite **Siųsti**.</span><span class="sxs-lookup"><span data-stu-id="53621-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="53621-115">Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo parametrų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="53621-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="53621-116">Veiksmus, kuriuos reikia patikrinti atšaukimo, ieškokite [šiame straipsnyje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="53621-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="53621-117">El. laiškų ieška ir naikinimas organizacijoje</span><span class="sxs-lookup"><span data-stu-id="53621-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="53621-118">Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į el. duomenų aptikimo tvarkytuvo vaidmenį arba atitikties ieškos valdymo vaidmenį, kad būtų ieškoma pranešimų.</span><span class="sxs-lookup"><span data-stu-id="53621-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="53621-119">Norėdami panaikinti pranešimus, turėsite prisijungti prie vaidmenų grupės Organizacijos valdymas arba ieškos ir valymo valdymo vaidmens.</span><span class="sxs-lookup"><span data-stu-id="53621-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="53621-120">Šių vaidmenų teisės priskiriamos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="53621-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="53621-121">[Sukurkite turinio iešką,](https://docs.microsoft.com/office365/securitycompliance/content-search) kad rastumėte naikintiną pranešimą.</span><span class="sxs-lookup"><span data-stu-id="53621-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="53621-122">[Prisijunkite prie saugos ir atitikties centro "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="53621-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="53621-123">Jei naudojate kelių dalių autentifikavimą, [žr.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="53621-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>