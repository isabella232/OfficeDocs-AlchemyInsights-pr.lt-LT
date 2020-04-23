---
title: Kaip išjungti išorines grupes
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720776"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="8f6b0-102">Kaip išjungti išorines grupes</span><span class="sxs-lookup"><span data-stu-id="8f6b0-102">How to disable External Groups</span></span>

<span data-ttu-id="8f6b0-103">"Yammer" išoriniai pranešimai taiko "Exchange" transportavimo taisykles (ETRs), aktyvių valdiklių rinkinį, kad įmonės informacija nebūtų bendrinama.</span><span class="sxs-lookup"><span data-stu-id="8f6b0-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="8f6b0-104">Norėdami apriboti vartotojų nuo išorinių grupių kūrimo, turite sukonfigūruoti "Exchange" transportavimo taisyklę (ETR), tada sukonfigūruoti "Yammer", kad "Exchange Transport" taisyklė būtų naudojama išoriniams pranešimams blokuoti.</span><span class="sxs-lookup"><span data-stu-id="8f6b0-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="8f6b0-105">Sukūrę taisyklę "Exchange Online" administravimo centre, atlikite šiuos veiksmus, kad nustatytumėte, ar ETR taikyti "Yammer":</span><span class="sxs-lookup"><span data-stu-id="8f6b0-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="8f6b0-106">Įeikite į "Yammer" kaip patvirtintas administratorius, o **"Yammer" administravimo centre**eikite į C **turinio ir saugos \> saugos parametrai.**</span><span class="sxs-lookup"><span data-stu-id="8f6b0-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="8f6b0-107">Dalyje **Išoriniai pranešimai**pasirinkite Įgalinti **"Exchange Online Exchange" transportavimo taisykles (ETR) "Yammer".**</span><span class="sxs-lookup"><span data-stu-id="8f6b0-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="8f6b0-108">Pasirinkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="8f6b0-108">Choose **Save**.</span></span>

<span data-ttu-id="8f6b0-109">Daugiau informacijos [ieškokite Išjungti išorinius pranešimus "Yammer" tinkle](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="8f6b0-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  