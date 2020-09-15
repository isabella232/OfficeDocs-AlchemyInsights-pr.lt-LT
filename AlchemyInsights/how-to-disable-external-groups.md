---
title: Kaip išjungti išorines grupes
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704136"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="eaf3f-102">Kaip išjungti išorines grupes</span><span class="sxs-lookup"><span data-stu-id="eaf3f-102">How to disable External Groups</span></span>

<span data-ttu-id="eaf3f-103">"Yammer" išoriniai pranešimai taiko "Exchange" transportavimo taisykles (ETRs), iniciatyvių valdiklių rinkinį, kad nebūtų bendrinama įmonės informacija.</span><span class="sxs-lookup"><span data-stu-id="eaf3f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="eaf3f-104">Kad vartotojai negalėtų sukurti išorinių grupių, turite sukonfigūruoti "Exchange" transportavimo taisyklę (ETR), tada Konfigūruokite "Yammer", kad galėtumėte naudoti "Exchange" transportavimo taisyklę, kad blokuotumėte išorinius pranešimus.</span><span class="sxs-lookup"><span data-stu-id="eaf3f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="eaf3f-105">Sukūrę taisyklę "Exchange Online" administravimo centre, atlikite šiuos veiksmus, kad nustatytumėte ETR, kad būtų taikoma "Yammer":</span><span class="sxs-lookup"><span data-stu-id="eaf3f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="eaf3f-106">Prisiregistruokite prie "Yammer" kaip patvirtintas administratorius ir " **Yammer" administravimo centre**eikite į C **turinys ir saugos \> Parametrai.**</span><span class="sxs-lookup"><span data-stu-id="eaf3f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="eaf3f-107">Dalyje **išoriniai pranešimai**pažymėkite **"Yammer" "Exchange Online" "Exchange" transportavimo taisyklės (etrs).**</span><span class="sxs-lookup"><span data-stu-id="eaf3f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="eaf3f-108">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="eaf3f-108">Choose **Save**.</span></span>

<span data-ttu-id="eaf3f-109">Daugiau informacijos rasite [išorinių pranešimų išjungimas "Yammer" tinkle](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="eaf3f-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  