---
title: 1554 Winsock klaida 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903112"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="946ac-102">Winsock klaida 10061</span><span class="sxs-lookup"><span data-stu-id="946ac-102">Winsock error 10061</span></span>

<span data-ttu-id="946ac-p101">Ši klaida reiškia, kad "Office 365" negalėjo sukurti TCP socket (jungtis) su tikslinės priimančiosios. Labiausiai tikėtina, dažniausia šios klaidos priežastis yra ugniasienės konfigūracijos problema. Norėdami išspręsti šią problemą, patikrinkite šiuos parametrus:</span><span class="sxs-lookup"><span data-stu-id="946ac-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="946ac-106">Patikrinkite, ar jūsų ugniasienės konfigūracijos informacija iš [Office 365 URL ir IP adresų diapazonas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="946ac-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="946ac-107">Jei klaidos yra susijusios su Exchange Online Protection (EOP), jums turėtų anksčiau pranešama apie pasikeičia į [Exchange Online apsaugos IP adresus](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="946ac-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="946ac-108">Įsitikinkite, kad jūsų interneto paslaugų teikėjas (ISP) neblokuoja uosto.</span><span class="sxs-lookup"><span data-stu-id="946ac-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="946ac-109">Patikrinkite, ar protingas pagrindinio kompiuterio ir paskirties serverio parametrus jūsų jungtys.</span><span class="sxs-lookup"><span data-stu-id="946ac-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="946ac-110">Atkreipkite dėmesį, kad "Office 365" ne blokuoti *priimamus* ryšius, tokiu būdu.</span><span class="sxs-lookup"><span data-stu-id="946ac-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

