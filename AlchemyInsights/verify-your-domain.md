---
title: Domeno tikrinimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710451"
---
# <a name="verify-your-domain"></a><span data-ttu-id="aa008-102">Domeno tikrinimas</span><span class="sxs-lookup"><span data-stu-id="aa008-102">Verify your domain</span></span>

 <span data-ttu-id="aa008-103">**Įrašas tikriausiai nebuvo atnaujintas visame internete.**</span><span class="sxs-lookup"><span data-stu-id="aa008-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="aa008-104">Paprastai mums reikia tik kelių minučių, kad galėtume pamatyti naują įrašą, tačiau kartais tai gali užtrukti tiek laiko, kiek kelias valandas.</span><span class="sxs-lookup"><span data-stu-id="aa008-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="aa008-105">Jei jau ilgai laukėte, dar kartą patikrinkite, ar nukopijavote ir įklijavote tikslią reikšmę į TXT patvirtinimo įrašą DNS išteklių nuomos teikėjo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="aa008-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="aa008-106">Viena dažniausia problema nėra įrašo dalis "MS=".</span><span class="sxs-lookup"><span data-stu-id="aa008-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="aa008-107">Mums to reikia!</span><span class="sxs-lookup"><span data-stu-id="aa008-107">We need that too!</span></span>

- <span data-ttu-id="aa008-108">Kai kuriuose DNS pagrindiniuose kompiuteriuose turite atlikti papildomą veiksmą, kad įrašytumėte zonos failą (kuriame saugomas DNS įrašas), kad jis būtų atnaujintas internete.</span><span class="sxs-lookup"><span data-stu-id="aa008-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="aa008-109">Įsitikinkite, kad įrašėte pakeitimus, kad "Microsoft" galėtų matyti ir patvirtinti įrašą.</span><span class="sxs-lookup"><span data-stu-id="aa008-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
