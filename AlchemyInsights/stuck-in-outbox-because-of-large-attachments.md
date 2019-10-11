---
title: Įstrigo Siunčidėžėje dėl didelių priedų
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441313"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="566b5-102">Pranešimų, kurie užstrigo Siunčidėžėje, taisymas</span><span class="sxs-lookup"><span data-stu-id="566b5-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="566b5-103">Mes rekomenduojame, kad jūs pradedate veikia scenarijų ["man kyla problemų siunčiant, gaunant arba ieškant el. laiškų"](https://aka.ms/SaRA-OutlookSendReceive) iš ["Microsoft" palaikymo ir atkūrimo asistentas](https://diagnostics.office.com/#/) įrankis.</span><span class="sxs-lookup"><span data-stu-id="566b5-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="566b5-104">Kai pranešimas užstrigo jūsų Siunčidėžėje, labiausiai tikėtina priežastis yra:</span><span class="sxs-lookup"><span data-stu-id="566b5-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="566b5-105">Dideli priedai.</span><span class="sxs-lookup"><span data-stu-id="566b5-105">Large attachments.</span></span>
- <span data-ttu-id="566b5-106">Į **Siųsti iš karto, kai prijungtas** parinktis neįgalintas.</span><span class="sxs-lookup"><span data-stu-id="566b5-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="566b5-107">Jei norite pašalinti didelius priedus:</span><span class="sxs-lookup"><span data-stu-id="566b5-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="566b5-108">Programoje "Outlook" pasirinkite **Siųsti/gauti** > **darbą neprisijungus**.</span><span class="sxs-lookup"><span data-stu-id="566b5-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="566b5-109">Naršymo srityje pasirinkite **siunčiama**.</span><span class="sxs-lookup"><span data-stu-id="566b5-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="566b5-110">Iš čia galite:</span><span class="sxs-lookup"><span data-stu-id="566b5-110">From here, you can:</span></span> 
    - <span data-ttu-id="566b5-111">Panaikinkite pranešimą (pažymėkite jį ir pasirinkite **Naikinti**).</span><span class="sxs-lookup"><span data-stu-id="566b5-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="566b5-112">Vilkite pranešimą į juodraščių aplanką, dukart spustelėkite, kad jį atidarytumėte, tada pašalinkite priedą ir pasirinkite jį, tada pasirinkite **Naikinti**).</span><span class="sxs-lookup"><span data-stu-id="566b5-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="566b5-113">Jei gaunate klaidos pranešimą, kuriame sakoma, kad "Outlook" bando perduoti žinutę, uždarykite programą "Outlook".</span><span class="sxs-lookup"><span data-stu-id="566b5-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="566b5-114">Tai gali užtrukti kelias akimirkas išeiti.</span><span class="sxs-lookup"><span data-stu-id="566b5-114">It may take a few moments to exit.</span></span> <span data-ttu-id="566b5-115">Jei "Outlook" neužsidaro, paspauskite CTRL + ALT + DELETE ir pasirinkite **paleisti užduočių tvarkytuvą**.</span><span class="sxs-lookup"><span data-stu-id="566b5-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="566b5-116">Užduočių tvarkytuve pasirinkite skirtuką **procesai** , slinkite žemyn iki "Outlook. exe" ir pasirinkite **Baigti procesą**.</span><span class="sxs-lookup"><span data-stu-id="566b5-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="566b5-117">Uždarius programą Outlook, paleiskite ją iš naujo ir pakartokite 2 ir 3 veiksmus.</span><span class="sxs-lookup"><span data-stu-id="566b5-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="566b5-118">Pašalinus priedą, spustelėkite **Siųsti/gauti** > **darbo neprisijungus** tęsti darbą internete.</span><span class="sxs-lookup"><span data-stu-id="566b5-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="566b5-119">Pranešimai taip pat įstrigti Siunčidėžėje spustelėjus **Siųsti**, bet nesate prisijungę.</span><span class="sxs-lookup"><span data-stu-id="566b5-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="566b5-120">Spustelėkite **Siųsti/gauti** ir pažiūrėkite į **darbo neprisijungus** mygtuką.</span><span class="sxs-lookup"><span data-stu-id="566b5-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="566b5-121">Jei jis mėlynas, atjungiate.</span><span class="sxs-lookup"><span data-stu-id="566b5-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="566b5-122">Pasirinkite, kad prisijungtumėte (mygtukas pasidaro baltas) ir spustelėkite **Siųsti viską**.</span><span class="sxs-lookup"><span data-stu-id="566b5-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="566b5-123">Jei norite įjungti **siuntimą iš karto, kai esate prisijungę**:</span><span class="sxs-lookup"><span data-stu-id="566b5-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="566b5-124">Pasirinkite **failų** > **parinktys** >  **Išplėstinės**.</span><span class="sxs-lookup"><span data-stu-id="566b5-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="566b5-125">Į į **Siųsti ir gauti** skyriuje, pasirinkite **Siųsti iš karto, kai prijungtas**, ir tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="566b5-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="566b5-126">Išsami informacija pateikiama:</span><span class="sxs-lookup"><span data-stu-id="566b5-126">For full details see:</span></span>
- [<span data-ttu-id="566b5-127">Vaizdo įrašas: nesuprantamos el. laiško siuntimas arba naikinimas</span><span class="sxs-lookup"><span data-stu-id="566b5-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="566b5-128">El. paštas lieka aplanke siunčiama, kol rankiniu būdu inicijuokite siuntimo/gavimo operaciją "Outlook"</span><span class="sxs-lookup"><span data-stu-id="566b5-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
