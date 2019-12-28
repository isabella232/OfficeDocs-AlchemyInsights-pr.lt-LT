---
title: Siųskite pasirinktinius pranešimus naudodami "Intune"
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886865"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="795cb-102">Kaip siųsti pasirinktinius pranešimus valdomų "iOS" ir "Android" įrenginių vartotojams</span><span class="sxs-lookup"><span data-stu-id="795cb-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="795cb-103">Pasirinktiniai pranešimai Intune apdorojami įmonės portalo programėlę vartotojo įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="795cb-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="795cb-104">Tada programėlė sukuria "Push" pranešimą tame įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="795cb-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="795cb-105">Toliau pateikiami įrenginio Būtinosios sąlygos, kad būtų galima gauti pasirinktinius pranešimus, ir programa, tada sukurti Push pranešimą:</span><span class="sxs-lookup"><span data-stu-id="795cb-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="795cb-106">Įrenginyje turi būti įdiegta įmonės portalo programėlė.</span><span class="sxs-lookup"><span data-stu-id="795cb-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="795cb-107">Įrenginys turi leisti įmonės portalo programai siųsti aktyviuosius pranešimus.</span><span class="sxs-lookup"><span data-stu-id="795cb-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="795cb-108">Kai programėlė bus įdiegta arba atnaujinta, ji paragins vartotoją leisti pranešimus.</span><span class="sxs-lookup"><span data-stu-id="795cb-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="795cb-109">"Android" įrenginiuose turi būti įdiegtos "Google Play" paslaugos.</span><span class="sxs-lookup"><span data-stu-id="795cb-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="795cb-110">Įrenginys turi būti įtrauktas į Intune.</span><span class="sxs-lookup"><span data-stu-id="795cb-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="795cb-111">Daugiau informacijos, įskaitant tai, kaip siųsti žinutę, ieškokite [funkcijų dokumentacijoje](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="795cb-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
