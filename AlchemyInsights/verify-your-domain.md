---
title: Domeno tikrinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770999"
---
# <a name="verify-your-domain"></a><span data-ttu-id="8f181-102">Domeno tikrinimas</span><span class="sxs-lookup"><span data-stu-id="8f181-102">Verify your domain</span></span>

 <span data-ttu-id="8f181-103">**Tikriausiai įrašas nebuvo atnaujintas internete.**</span><span class="sxs-lookup"><span data-stu-id="8f181-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="8f181-104">Paprastai mums užtrunka tik kelios minutės, kol galėsime matyti naują įrašą, tačiau kartais tai gali užtrukti iki kelių valandų.</span><span class="sxs-lookup"><span data-stu-id="8f181-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="8f181-105">Jei jau ilgai laukėte, dukart patikrinkite, ar nukopijavote ir įklijuojate tikslią reikšmę į TXT patvirtinimo įrašą DNS išteklių nuomos teikėjo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="8f181-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="8f181-106">Viena dažniausia problema nėra įrašo dalis "MS=".</span><span class="sxs-lookup"><span data-stu-id="8f181-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="8f181-107">Mums to taip pat reikia!</span><span class="sxs-lookup"><span data-stu-id="8f181-107">We need that too!</span></span>

- <span data-ttu-id="8f181-108">Kai kuriuose DNS išteklių nuomos teikėjose turite atlikti papildomą veiksmą, kad įrašytumėte zonos failą (kur saugomas DNS įrašas), kad jis būtų naujinys internete.</span><span class="sxs-lookup"><span data-stu-id="8f181-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="8f181-109">Įsitikinkite, kad įrašėte keitimus, kad "Microsoft" galėtų peržiūrėti ir patvirtinti įrašą.</span><span class="sxs-lookup"><span data-stu-id="8f181-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
