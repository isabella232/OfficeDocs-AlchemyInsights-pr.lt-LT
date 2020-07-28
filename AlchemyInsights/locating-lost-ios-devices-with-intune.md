---
title: Prarastų "iOS" įrenginių radimas naudojant "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439630"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="1baf7-102">Prarastų "iOS" įrenginių radimas naudojant "Intune"</span><span class="sxs-lookup"><span data-stu-id="1baf7-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="1baf7-103">Įjungus prarastą režimą "iOS" įrenginyje, administratorius gali užrakto ekrane rodyti pranešimą ir kontaktinį telefono numerį.</span><span class="sxs-lookup"><span data-stu-id="1baf7-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="1baf7-104">Įjungus prarastą režimą, administratorius gali naudoti veiksmą Rasti įrenginį, kad nustatytų fizinę įrenginio vietą.</span><span class="sxs-lookup"><span data-stu-id="1baf7-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="1baf7-105">"Intune" veiksmas Rasti įrenginį veikia su "iOS" įrenginiais, kad žemėlapyje būtų rodoma konkretaus įrenginio vieta.</span><span class="sxs-lookup"><span data-stu-id="1baf7-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="1baf7-106">Norint atlikti šį veiksmą, reikia, kad "iOS" įrenginys būtų:</span><span class="sxs-lookup"><span data-stu-id="1baf7-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="1baf7-107">Prižiūrimas režimas</span><span class="sxs-lookup"><span data-stu-id="1baf7-107">Supervised mode</span></span>
- <span data-ttu-id="1baf7-108">Prarastas režimas</span><span class="sxs-lookup"><span data-stu-id="1baf7-108">Lost mode</span></span>

<span data-ttu-id="1baf7-109">Daugiau informacijos rasite ["iOS" / "iPadOS" įrenginiuose su "Intune" įjungta prarastu režimu](https://docs.microsoft.com/intune/device-lost-mode) ir [raskite pamestus ar pavogtus "iOS" / "iPadOS" įrenginius su "Intune" įrenginiais.](https://docs.microsoft.com/intune/device-locate)</span><span class="sxs-lookup"><span data-stu-id="1baf7-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="1baf7-110">**DUK**</span><span class="sxs-lookup"><span data-stu-id="1baf7-110">**FAQ**</span></span>

<span data-ttu-id="1baf7-111">Klausimas: Aš išleido nuotolinio veiksmų pašalinti įmonės duomenis iš įrenginio, ir dabar jis įstrigo laukiančioje būsenoje.</span><span class="sxs-lookup"><span data-stu-id="1baf7-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="1baf7-112">A: Kad nuotolinis veiksmas būtų sėkmingai užbaigtas, tikslinis įrenginys turi būti internete ir sveikas.</span><span class="sxs-lookup"><span data-stu-id="1baf7-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="1baf7-113">Toliau nurodytais atvejais nuotolinis veiksmas lieka laukiančioje būsenoje 30 dienų arba tol, kol įrenginys patvirtina komandą:</span><span class="sxs-lookup"><span data-stu-id="1baf7-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="1baf7-114">Kai prietaisas neturi ryšio su</span><span class="sxs-lookup"><span data-stu-id="1baf7-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="1baf7-115">Kai prietaisas praranda valdymo būseną su Intune</span><span class="sxs-lookup"><span data-stu-id="1baf7-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="1baf7-116">Jei manote, kad įrenginys nebeprisiregistruoja ir negalės pašalinti įmonės duomenų, pasirinkite Naikinti.</span><span class="sxs-lookup"><span data-stu-id="1baf7-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="1baf7-117">Panaikinus įrenginio įrašą pašalinamas, kad jis nebebūtų rodomas įrenginių sąraše Intune.</span><span class="sxs-lookup"><span data-stu-id="1baf7-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="1baf7-118">Jei įrenginys vėl įsijungia, jo vartotojas turės jį užregistruoti iš naujo.</span><span class="sxs-lookup"><span data-stu-id="1baf7-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="1baf7-119">Klausimas: Kodėl tam tikrų nuotolinių veiksmų negalima naudoti?</span><span class="sxs-lookup"><span data-stu-id="1baf7-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="1baf7-120">A: Ne visos platformos palaiko visus nuotolinio įrenginio veiksmus.</span><span class="sxs-lookup"><span data-stu-id="1baf7-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="1baf7-121">Šie nuotoliniai veiksmai yra susiję su platforma, todėl jie pasiekiami tik pažymėtiems platformoms.</span><span class="sxs-lookup"><span data-stu-id="1baf7-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="1baf7-122">Apeiti aktyvinimo užraktą (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="1baf7-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="1baf7-123">Nauja pradžia (tik "Windows")</span><span class="sxs-lookup"><span data-stu-id="1baf7-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="1baf7-124">Prarastas režimas (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="1baf7-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="1baf7-125">Įrenginio radimas (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="1baf7-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="1baf7-126">Paleisti iš naujo (tik "Windows")</span><span class="sxs-lookup"><span data-stu-id="1baf7-126">Restart (Windows only)</span></span>

<span data-ttu-id="1baf7-127">Daugiau informacijos apie kiekvieną veiksmą ieškokite [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="1baf7-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>