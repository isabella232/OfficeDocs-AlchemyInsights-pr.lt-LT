---
title: Darbas su "iOS" VPP taikomųjų programų id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719965"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="c90a8-102">Darbas su "iOS" VPP programomis</span><span class="sxs-lookup"><span data-stu-id="c90a8-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="c90a8-103">Skaitykite [Kaip valdyti "iOS" programėles, įsigytas naudojant tomo pirkimo programą su "Microsoft Intune",](https://docs.microsoft.com/intune/vpp-apps-ios) kad sužinotumėte apie funkcijas, apribojimus ir veiksmus, kaip pasinaudoti "Apple Volume Purchase" programa ir jos palaikymu programoje "Microsoft Intune".</span><span class="sxs-lookup"><span data-stu-id="c90a8-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="c90a8-104">**Dažniausiai pasitaikančios problemos:** "Priskiriau "iOS VPP" programą savo vartotojams, bet diegimas nepavyko."</span><span class="sxs-lookup"><span data-stu-id="c90a8-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="c90a8-105">Taip gali nutikti, jei keliuose mobiliųjų įrenginių valdymo paslaugų teikėjuose naudojamas vienas VPP atpažinimo ženklas.</span><span class="sxs-lookup"><span data-stu-id="c90a8-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="c90a8-106">VPP atpažinimo ženklus iš "Apple" galima naudoti tik su vienu teikėju.</span><span class="sxs-lookup"><span data-stu-id="c90a8-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="c90a8-107">Jei naudojote VPP atpažinimo ženklą su keliais teikėjais, turite iš naujo nusiųsti atpažinimo ženklą į Intune.</span><span class="sxs-lookup"><span data-stu-id="c90a8-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="c90a8-108">Diegimas taip pat gali nepavykti, jei bendras įrenginių skaičius viršija licencijų skaičių.</span><span class="sxs-lookup"><span data-stu-id="c90a8-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="c90a8-109">Norėdami peržiūrėti licencijų naudojimo ataskaitą, eikite į puslapį **"Intune Mobile Apps"** \> **licencijos.**</span><span class="sxs-lookup"><span data-stu-id="c90a8-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="c90a8-110">Norėdami sužinoti, kaip susigrąžinti naudojamas licencijas, skaitykite [šį straipsnį.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="c90a8-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
