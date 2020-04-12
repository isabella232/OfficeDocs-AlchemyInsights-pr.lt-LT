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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232638"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b6c6c-102">Pranešimų, kurie įstrigo aplanke Siunčiama, taisymas</span><span class="sxs-lookup"><span data-stu-id="b6c6c-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b6c6c-103">Rekomenduojame pradėti vykdyti scenarijų ["Kyla problemų siunčiant, gaunant arba ieškant el. laiškų"](https://aka.ms/SaRA-OutlookSendReceive) iš ["Microsoft" palaikymo ir atkūrimo asistentas](https://diagnostics.office.com/#/) įrankis susijusio kompiuterio.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="b6c6c-104">Kai pranešimas įstringa aplanke Siunčiama, labiausiai tikėtina priežastis yra didelis priedas arba parinktis "Siųsti iš karto prisijungus" neįgalinta.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b6c6c-105">**Pašalinti didelį priedą**</span><span class="sxs-lookup"><span data-stu-id="b6c6c-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b6c6c-106">Spustelėkite **Siųsti / gauti** > **darbą neprisijungus**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b6c6c-107">Naršymo srityje spustelėkite **Siunčiama**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="b6c6c-108">Iš čia galite:</span><span class="sxs-lookup"><span data-stu-id="b6c6c-108">From here, you can:</span></span> 
    - <span data-ttu-id="b6c6c-109">Panaikinkite pranešimą.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-109">Delete the message.</span></span> <span data-ttu-id="b6c6c-110">Tiesiog pažymėkite jį ir spustelėkite **Naikinti**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="b6c6c-111">Vilkite pranešimą į **juodraščių aplanką**, dukart spustelėkite, kad atidarytumėte pranešimą, ir panaikinkite priedą (spustelėkite jį ir spustelėkite **Naikinti**).</span><span class="sxs-lookup"><span data-stu-id="b6c6c-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="b6c6c-112">Jei klaida nurodo, kad "Outlook" bando perduoti pranešimą, uždarykite "Outlook".</span><span class="sxs-lookup"><span data-stu-id="b6c6c-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b6c6c-113">Gali praeiti kelios akimirkos.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-113">It may take a few moments to exit.</span></span> <span data-ttu-id="b6c6c-114">Jei "Outlook" neužsidaro, paspauskite **Ctrl + Alt + Delete** ir spustelėkite Paleisti **užduočių tvarkytuvą**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="b6c6c-115">Užduočių tvarkytuve pasirinkite skirtuką **Procesai,** slinkite žemyn iki outlook.exe ir spustelėkite **Baigti procesą**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="b6c6c-116">Kai "Outlook" uždaroma, iš naujo paleiskite "Outlook" ir pakartokite veiksmus 2-3.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="b6c6c-117">Pašalinę priedą, spustelėkite **Siųsti / gauti** > **darbą neprisijungus,** kad atšauktumėte mygtuko pasirinkimą ir tęstumėte darbą internete.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="b6c6c-118">Pranešimai taip pat įstrigo aplanke Siunčiama spustelėjus **Siųsti**, bet nesate prisijungę.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b6c6c-119">Spustelėkite **Siųsti / gauti** ir peržiūrėkite mygtuką Dirbti **neprisijungus.**</span><span class="sxs-lookup"><span data-stu-id="b6c6c-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b6c6c-120">Jei jis mėlynas, būsite atjungtas.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b6c6c-121">Spustelėkite jį, kad prisijungtumėte (mygtukas tampa baltas) ir spustelėkite **Siųsti viską**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b6c6c-122">**Įgalinti siųsti iš karto prisijungus**</span><span class="sxs-lookup"><span data-stu-id="b6c6c-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b6c6c-123">Skirtuke Failas spustelėkite **Parinktys**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b6c6c-124">Dialogo lange "Outlook" parinktys spustelėkite **Išsamiau**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b6c6c-125">Sekcijoje Siųsti ir gauti spustelėkite, kad įgalintumėte **Siųsti iš karto, kai prijungta .**</span><span class="sxs-lookup"><span data-stu-id="b6c6c-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b6c6c-126">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="b6c6c-126">Click **OK**.</span></span>
 
<span data-ttu-id="b6c6c-127">Išsamesnė informacija pateikiama:</span><span class="sxs-lookup"><span data-stu-id="b6c6c-127">For full details, see:</span></span>
- [<span data-ttu-id="b6c6c-128">Vaizdo įrašas: įstrigusio el. laiško siuntimas arba naikinimas</span><span class="sxs-lookup"><span data-stu-id="b6c6c-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b6c6c-129">El. paštas lieka aplanke Siunčiama, kol rankiniu būdu inicijuojate siuntimo/gavimo operaciją programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="b6c6c-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
