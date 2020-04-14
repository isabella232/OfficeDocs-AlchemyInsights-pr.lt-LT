---
title: Įstrigo aplanke Siunčiama dėl didelių priedų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241260"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="ede83-102">Pranešimų, kurie įstrigo aplanke Siunčiama, taisymas</span><span class="sxs-lookup"><span data-stu-id="ede83-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="ede83-103">Rekomenduojame pradėti vykdyti scenarijų ["Kyla problemų siunčiant, gaunant arba ieškant el. laiškų"](https://aka.ms/SaRA-OutlookSendReceive) iš ["Microsoft" palaikymo ir atkūrimo asistentas](https://diagnostics.office.com/#/) įrankis.</span><span class="sxs-lookup"><span data-stu-id="ede83-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="ede83-104">Kai pranešimas įstringa aplanke Siunčiama, labiausiai tikėtina priežastis yra didelis priedas arba parinktis "Siųsti iš karto prisijungus" neįgalinta.</span><span class="sxs-lookup"><span data-stu-id="ede83-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="ede83-105">**Pašalinti didelį priedą**</span><span class="sxs-lookup"><span data-stu-id="ede83-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="ede83-106">Programoje "Outlook" pasirinkite **Siųsti / gauti** > **darbą neprisijungus**.</span><span class="sxs-lookup"><span data-stu-id="ede83-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="ede83-107">Naršymo srityje pasirinkite **Siunčiama**.</span><span class="sxs-lookup"><span data-stu-id="ede83-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="ede83-108">Iš čia galite:</span><span class="sxs-lookup"><span data-stu-id="ede83-108">From here, you can:</span></span> 
    - <span data-ttu-id="ede83-109">I¹trinti prane¹im± (pasirinkite jç ir pasirinkite **I¹trinti**).</span><span class="sxs-lookup"><span data-stu-id="ede83-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="ede83-110">Vilkite pranešimą į aplanką Juodraščiai, dukart spustelėkite, kad jį atidarytumėte, ir pašalinkite priedą, pasirinkite jį, tada pasirinkite **Naikinti**).</span><span class="sxs-lookup"><span data-stu-id="ede83-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="ede83-111">Jei gaunate klaidos pranešimą, kuris sako, kad "Outlook" bando perduoti pranešimą, uždarykite "Outlook".</span><span class="sxs-lookup"><span data-stu-id="ede83-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="ede83-112">Gali praeiti kelios akimirkos.</span><span class="sxs-lookup"><span data-stu-id="ede83-112">It may take a few moments to exit.</span></span> <span data-ttu-id="ede83-113">Jei "Outlook" neužsidaro, paspauskite Ctrl + Alt + Delete ir pasirinkite **Paleisti užduočių tvarkytuvą**.</span><span class="sxs-lookup"><span data-stu-id="ede83-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="ede83-114">Užduočių tvarkytuve pasirinkite skirtuką **Procesai,** slinkite žemyn iki outlook.exe ir pasirinkite **Baigti procesą**.</span><span class="sxs-lookup"><span data-stu-id="ede83-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="ede83-115">Kai "Outlook" uždaroma, paleiskite jį iš naujo ir pakartokite 2 ir 3 veiksmus.</span><span class="sxs-lookup"><span data-stu-id="ede83-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="ede83-116">Pašalinę priedą, spustelėkite **Siųsti / gauti** > **darbą neprisijungus,** kad tęstumėte darbą tinkle.</span><span class="sxs-lookup"><span data-stu-id="ede83-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="ede83-117">Pranešimai taip pat įstrigo aplanke Siunčiama spustelėjus **Siųsti**, bet nesate prisijungę.</span><span class="sxs-lookup"><span data-stu-id="ede83-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="ede83-118">Spustelėkite **Siųsti / gauti** ir peržiūrėkite mygtuką Dirbti **neprisijungus.**</span><span class="sxs-lookup"><span data-stu-id="ede83-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="ede83-119">Jei jis mėlynas, būsite atjungtas.</span><span class="sxs-lookup"><span data-stu-id="ede83-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="ede83-120">Spustelėkite jį, kad prisijungtumėte (mygtukas tampa baltas) ir spustelėkite **Siųsti viską**.</span><span class="sxs-lookup"><span data-stu-id="ede83-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="ede83-121">**Įgalinti siųsti iš karto prisijungus**</span><span class="sxs-lookup"><span data-stu-id="ede83-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="ede83-122">Skirtuke Failas spustelėkite **Parinktys**.</span><span class="sxs-lookup"><span data-stu-id="ede83-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="ede83-123">Dialogo lange "Outlook" parinktys spustelėkite **Išsamiau**.</span><span class="sxs-lookup"><span data-stu-id="ede83-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="ede83-124">Sekcijoje Siųsti ir gauti spustelėkite, kad įgalintumėte **Siųsti iš karto, kai prijungta .**</span><span class="sxs-lookup"><span data-stu-id="ede83-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="ede83-125">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="ede83-125">Click **OK**.</span></span>
 
<span data-ttu-id="ede83-126">Išsamesnė informacija pateikiama:</span><span class="sxs-lookup"><span data-stu-id="ede83-126">For full details, see:</span></span>
- [<span data-ttu-id="ede83-127">Vaizdo įrašas: įstrigusio el. laiško siuntimas arba naikinimas</span><span class="sxs-lookup"><span data-stu-id="ede83-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="ede83-128">El. paštas lieka aplanke Siunčiama, kol rankiniu būdu inicijuojate siuntimo/gavimo operaciją programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="ede83-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
