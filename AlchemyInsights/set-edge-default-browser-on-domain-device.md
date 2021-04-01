---
title: "\"Microsoft Edge\" nustatymas kaip numatytosios naršyklės domeno įrenginyje"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491885"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="7bc37-102">"Microsoft Edge" nustatymas kaip numatytosios naršyklės domeno įrenginyje</span><span class="sxs-lookup"><span data-stu-id="7bc37-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="7bc37-103">Nustatykite "Microsoft Edge" kaip numatytąją naršyklę:</span><span class="sxs-lookup"><span data-stu-id="7bc37-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="7bc37-104">[Sukurkite numatytąjį susiejimų konfigūracijos](https://go.microsoft.com/fwlink/?linkid=2132437) failą ir laikykite jį vietoje arba bendrai naudojamas tinkle.</span><span class="sxs-lookup"><span data-stu-id="7bc37-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="7bc37-105">Atidarykite grupės strategijos rengyklę, tada eikite į **Kompiuterio konfigūravimo**  >  **administravimo šablonai**  >  **"Windows" komponentų**  >  **failų naršyklė**.</span><span class="sxs-lookup"><span data-stu-id="7bc37-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="7bc37-106">Pasirinkite **Nustatyti numatytąjį susiejimų konfigūracijos failą**.</span><span class="sxs-lookup"><span data-stu-id="7bc37-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="7bc37-107">Pasirinkite **Strategijos parametras**, tada pasirinkite **Įgalinta**.</span><span class="sxs-lookup"><span data-stu-id="7bc37-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="7bc37-108">Dalyje **Parinktys** įveskite numatytojo susiejimo konfigūracijos failo vietą, tada pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="7bc37-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
