---
title: Trikčių šalinimo saugos patarimas dėl sukčiavimo tikrina
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391217"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ffd49-102">Trikčių šalinimo saugos patarimas dėl sukčiavimo tikrina</span><span class="sxs-lookup"><span data-stu-id="ffd49-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="ffd49-103">Jei esate gauti saugos patarimas, sako "siuntėjo nepavyko mūsų sukčiavimo aptikimo patikrinimus ir gali nebūti tais, kuo jie gali būti", tada siuntėjo nesugebėjo perduoti DKIM arba SPF autentiškumo tikrinimus.</span><span class="sxs-lookup"><span data-stu-id="ffd49-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ffd49-104">Geriausias būdas išspręsti šią problemą yra siuntėjui leisti save.</span><span class="sxs-lookup"><span data-stu-id="ffd49-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ffd49-105">Jei siuntėjas siunčia jūsų vardu, jums reikia leisti juos įtraukus siuntėjo IP adresą į savo SPF įrašą.</span><span class="sxs-lookup"><span data-stu-id="ffd49-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ffd49-106">Žiūrėkite [trikčių šalinimo raudona (įtartinų) saugos patarimas dėl sukčiavimo tikrina](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) daugiau info.</span><span class="sxs-lookup"><span data-stu-id="ffd49-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="ffd49-107">Čia yra keletas kitų nuorodų, kurios gali padėti:</span><span class="sxs-lookup"><span data-stu-id="ffd49-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ffd49-108">Kaip "Office 365" naudoja siuntėjo strategijos sistemą (SPF) užkirsti kelią parodijos</span><span class="sxs-lookup"><span data-stu-id="ffd49-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="ffd49-109">Nustatyti SPF "Office 365", Norėdami apsisaugoti nuo apsimetimo kitu</span><span class="sxs-lookup"><span data-stu-id="ffd49-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

