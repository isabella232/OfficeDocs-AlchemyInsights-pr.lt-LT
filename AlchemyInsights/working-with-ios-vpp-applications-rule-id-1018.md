---
title: Darbo su "iOS" VPP programos taisyklė Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480715"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="444e7-102">Darbas su "iOS" VPP programos</span><span class="sxs-lookup"><span data-stu-id="444e7-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="444e7-103">Skaitykite, [kaip valdyti įsigytos apimties pirkimo programą su Microsoft Intune "iOS" programos](https://docs.microsoft.com/intune/vpp-apps-ios) sužinoti apie funkcijas, apribojimų ir priemonių, kad naudoti Apple apimties pirkimo programa ir parama už jį į Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="444e7-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="444e7-104">**Bendrų klausimų:** "Paskyriau VPP programėlė" iOS "vartotojai, tačiau įdiegti nepavyko."</span><span class="sxs-lookup"><span data-stu-id="444e7-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="444e7-p101">Tai gali atsitikti, jei bendrosios VPP žetonas naudojamas visoje kelis mobiliojo prietaiso valdymo paslaugų teikėjus. VPP žetonų iš Apple gali būti tik su vienu tiekėju. Jei naudojote VPP atpažinimo ženklas su keliais paslaugų teikėjais, jūs turi iš naujo įkelti atpažinimo ženklo Intune.</span><span class="sxs-lookup"><span data-stu-id="444e7-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="444e7-p102">Įrenginys taip pat gali nepasisekti, jei bendras įrenginių skaičius viršija licencijų skaičiaus. Jei norite peržiūrėti naudojimo ataskaitą už savo licencijas, eikite į **Intune mobiliųjų programėlių** \> **programėlių licencijas** puslapis. Norėdami sužinoti kaip susigrąžinti licencijų naudojimą, žiūrėkite [šio straipsnio.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="444e7-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

