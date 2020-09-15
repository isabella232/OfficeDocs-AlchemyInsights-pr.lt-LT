---
title: Darbas su "iOS" VPP taikomųjų programų taisyklės ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688954"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="4ee8f-102">Darbas su "iOS" VPP programomis</span><span class="sxs-lookup"><span data-stu-id="4ee8f-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="4ee8f-103">Skaitykite, [kaip tvarkyti "iOS" taikomąsias programas, įsigytas naudojant tomo pirkimo programą su "Microsoft Intune"](https://docs.microsoft.com/intune/vpp-apps-ios) , Norėdami sužinoti apie funkcijas, apribojimus ir veiksmus, kad naudotumėte "Apple" tomo įsigijimo programą ir jos palaikymą programoje "Microsoft Intune".</span><span class="sxs-lookup"><span data-stu-id="4ee8f-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="4ee8f-104">**Dažnai pasitaikančių problemų:** "Aš paskyrę" iOS "VPP programėlę savo vartotojams, bet nepavyko įdiegti."</span><span class="sxs-lookup"><span data-stu-id="4ee8f-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="4ee8f-105">Taip gali nutikti, jei vienas VPP ženklas naudojamas keliuose mobiliųjų įrenginių valdymo paslaugų teikėjams.</span><span class="sxs-lookup"><span data-stu-id="4ee8f-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="4ee8f-106">"Apple" VPP žetonų galima naudoti tik su vienu tiekėju.</span><span class="sxs-lookup"><span data-stu-id="4ee8f-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="4ee8f-107">Jei naudojote VPP atpažinimo ženklą su keliais teikėjais, turite iš naujo nusiųsti atpažinimo ženklą į Intune.</span><span class="sxs-lookup"><span data-stu-id="4ee8f-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="4ee8f-108">Diegimas taip pat gali nepavykti, jei bendras įrenginių skaičius viršija licencijų skaičių.</span><span class="sxs-lookup"><span data-stu-id="4ee8f-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="4ee8f-109">Norėdami peržiūrėti savo licencijų naudojimo ataskaitą, eikite į "Intune" **mobiliųjų įrenginių taikomųjų** programų \> **licencijų** puslapį.</span><span class="sxs-lookup"><span data-stu-id="4ee8f-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="4ee8f-110">Norėdami sužinoti, kaip panaudoti licencijų naudojimą, skaitykite [šį straipsnį.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="4ee8f-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
