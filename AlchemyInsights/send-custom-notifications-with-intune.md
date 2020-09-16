---
title: Pasirinktinio pranešimų siuntimas naudojant "Intune"
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720654"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="febba-102">Kaip nusiųsti pritaikytus pranešimus valdomoms "iOS" ir "Android" įrenginiams vartotojams</span><span class="sxs-lookup"><span data-stu-id="febba-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="febba-103">Pasirinktinio naudojimo pranešimus, skirtus "Intune", tvarko įmonės portalo programėlė vartotojo įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="febba-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="febba-104">Tada programa sukuria "Push" pranešimą tame įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="febba-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="febba-105">Toliau nurodyti įrenginio Būtinosios sąlygos, skirtos palaikyti pasirinktiniams pranešimams gavimą, o tada programėlei sukurti "Push" pranešimą:</span><span class="sxs-lookup"><span data-stu-id="febba-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="febba-106">Įrenginyje turi būti įdiegta įmonės portalo taikomoji programa.</span><span class="sxs-lookup"><span data-stu-id="febba-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="febba-107">Įrenginys turi leisti įmonės portalo taikomajai programai išsiųsti "Push" pranešimus.</span><span class="sxs-lookup"><span data-stu-id="febba-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="febba-108">Kai taikomoji programa įdiegiama arba atnaujinama, ji paragins vartotoją leisti pranešimus.</span><span class="sxs-lookup"><span data-stu-id="febba-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="febba-109">"Android" įrenginiuose turi būti įdiegtos "Google Play" paslaugos.</span><span class="sxs-lookup"><span data-stu-id="febba-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="febba-110">Įrenginys turi būti užregistruotas su Intune.</span><span class="sxs-lookup"><span data-stu-id="febba-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="febba-111">Daugiau informacijos, įskaitant pranešimo siuntimą, rasite [funkcijų dokumentacijoje](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="febba-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
