---
title: Konvertuoti vartotojo pašto dėžutės į bendrinamą pašto dėžutę?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496443"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="d0f25-102">Konvertuoti į bendrai naudojamos pašto dėžutės vartotojo pašto dėžutė</span><span class="sxs-lookup"><span data-stu-id="d0f25-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="d0f25-103">Tik galite konvertuoti vartotojo pašto dėžutės bendrinamos pašto dėžutės jei vartotojas turi keistis licenciją.</span><span class="sxs-lookup"><span data-stu-id="d0f25-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="d0f25-104">Konvertavus į pašto dėžutę, ji ir toliau bus rodomi į aktyvių vartotojų sąrašą, nes tame sąraše yra bendrai naudojamos pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="d0f25-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="d0f25-105">Vis dėlto konvertuoti pašto dėžutės taip pat pasirodys sąraše bendrai naudojamos pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="d0f25-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d0f25-106">Jei bandysite konvertuoti pašto dėžutės Exchange administratoriaus konsolėje ir konvertavimo nepavyksta, išvalykite naršyklės talpyklą ir slapukus, ir bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="d0f25-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="d0f25-107">Jei vis tiek neveikia, bandykite konvertuoti pašto dėžutės Exchange valdymo aplinkoje vykdydami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="d0f25-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d0f25-108">Daugiau pašto dėžučių konvertavimas informacija pateikiama [konvertuoti bendrinamos pašto dėžutės vartotojo pašto dėžutės](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d0f25-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
