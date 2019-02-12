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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906740"
---
<span data-ttu-id="35184-p101">Tik galite konvertuoti vartotojo pašto dėžutės bendrinamos pašto dėžutės jei vartotojas turi keistis licenciją. Konvertavus į pašto dėžutę, ji ir toliau bus rodomi į aktyvių vartotojų sąrašą, nes tame sąraše yra bendrai naudojamos pašto dėžutės. Vis dėlto konvertuoti pašto dėžutės taip pat pasirodys sąraše bendrai naudojamos pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="35184-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="35184-p102">Jei bandysite konvertuoti pašto dėžutės Exchange administratoriaus konsolėje ir konvertavimo nepavyksta, išvalykite naršyklės talpyklą ir slapukus, ir bandykite dar kartą. Jei vis tiek neveikia, bandykite konvertuoti pašto dėžutės Exchange valdymo aplinkoje vykdydami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="35184-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="35184-107">Daugiau pašto dėžučių konvertavimas informacija pateikiama [konvertuoti bendrinamos pašto dėžutės vartotojo pašto dėžutės](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="35184-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
