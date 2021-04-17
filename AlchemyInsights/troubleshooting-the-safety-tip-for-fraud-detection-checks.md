---
title: Apgaulės aptikimo tikrinimo saugos patarimo trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834739"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="9166b-102">Apgaulės aptikimo tikrinimo saugos patarimo trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="9166b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="9166b-103">Jei gaunate saugos patarimą, kuriame rašoma: "Siuntėjui nepavyko aptikti sukčiavimo ir jis gali būti ne toks, kaip jis atrodo", siuntėjui nepavyko atlikti DKIM arba SPF autentifikavimo patikrų.</span><span class="sxs-lookup"><span data-stu-id="9166b-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="9166b-104">Geriausias būdas išspręsti šią problemą yra leisti siuntėjui.</span><span class="sxs-lookup"><span data-stu-id="9166b-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="9166b-105">Jei siuntėjas siunčia jūsų vardu, turite jį autorizuoti įtraukdami siuntėjo IP adresą į SAVO SPF įrašą.</span><span class="sxs-lookup"><span data-stu-id="9166b-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="9166b-106">Daugiau [informacijos žr. Raudono (įtartinos) saugos patarimo trikčių](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) šalinimas, kad būtų galima aptikti apgaulės atvejus.</span><span class="sxs-lookup"><span data-stu-id="9166b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="9166b-107">Štai keletas kitų saitų, kurie gali padėti:</span><span class="sxs-lookup"><span data-stu-id="9166b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="9166b-108">Kaip "Microsoft" naudoja siuntėjų strategijos sistemą (SPF), kad išvengtų sąsojimo</span><span class="sxs-lookup"><span data-stu-id="9166b-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="9166b-109">SPF, kad būtų užkirstas kelias spoofing</span><span class="sxs-lookup"><span data-stu-id="9166b-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
