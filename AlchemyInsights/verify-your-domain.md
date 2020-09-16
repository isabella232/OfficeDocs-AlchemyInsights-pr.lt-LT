---
title: Domeno tikrinimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734314"
---
# <a name="verify-your-domain"></a><span data-ttu-id="413c0-102">Domeno tikrinimas</span><span class="sxs-lookup"><span data-stu-id="413c0-102">Verify your domain</span></span>

 <span data-ttu-id="413c0-103">**Įrašas tikriausiai neatnaujintas internete.**</span><span class="sxs-lookup"><span data-stu-id="413c0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="413c0-104">Paprastai, kad galėtume matyti naują įrašą, tačiau kartais gali užtrukti kelias valandas, nes tai gali užtrukti keletą minučių.</span><span class="sxs-lookup"><span data-stu-id="413c0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="413c0-105">Jei dar ilgai laukėte, dar kartą patikrinkite, ar nukopijavote ir įklijavote tikslią reikšmę į TXT patvirtinimo įrašą savo DNS išteklių nuomos teikėjo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="413c0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="413c0-106">Viena dažniausių problemų nėra įtraukiant "MS =" įrašo dalį.</span><span class="sxs-lookup"><span data-stu-id="413c0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="413c0-107">Turime taip pat!</span><span class="sxs-lookup"><span data-stu-id="413c0-107">We need that too!</span></span>

- <span data-ttu-id="413c0-108">Kai kuriuose DNS pagrindiniuose kompiuteriuose turite atlikti papildomą veiksmą, kad įrašytumėte zonos failą (kur saugomas DNS įrašas), kad jis būtų atnaujintas internete.</span><span class="sxs-lookup"><span data-stu-id="413c0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="413c0-109">Įsitikinkite, kad įrašėte savo atliktus įrašus, kad "Microsoft" galėtų matyti ir patvirtinti įrašą.</span><span class="sxs-lookup"><span data-stu-id="413c0-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
