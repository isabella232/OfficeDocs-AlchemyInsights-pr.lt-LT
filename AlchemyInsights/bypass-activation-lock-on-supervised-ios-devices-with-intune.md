---
title: Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424219"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="ed6c6-102">Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune"</span><span class="sxs-lookup"><span data-stu-id="ed6c6-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="ed6c6-103">Galimybė apeiti aktyvinimo užraktą "iOS" įrenginiuose leidžia lengviau atsigauti pagal scenarijų, kai vartotojas įgalina aktyvinimo užraktą įmonės įrenginyje, o tada palieka įmonę.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="ed6c6-104">Išankstinės aktyvinimo užrakto apėjimo sąlygos:</span><span class="sxs-lookup"><span data-stu-id="ed6c6-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="ed6c6-105">Įrenginys yra "prižiūrimas".</span><span class="sxs-lookup"><span data-stu-id="ed6c6-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="ed6c6-106">Aktyvinimo užraktas sėkmingai įgalintas naudojant "iOS" įrenginio apribojimo strategiją in Intune.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="ed6c6-107">Be to, apeinant aktyvinimo užraktą turėtumėte:</span><span class="sxs-lookup"><span data-stu-id="ed6c6-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="ed6c6-108">Fiziškai turėti prietaisą nušluostyti.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="ed6c6-109">Nukopijuokite kodą prieš išduokite ištrynimą.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="ed6c6-110">**Pastaba:** Valymo kodas nėra didžiosios ir mažosios raidės, todėl "-" simbolių nereikia.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="ed6c6-111">Daugiau informacijos rasite [Apeiti aktyvinimo užraktą prižiūrimuose "iOS" įrenginiuose su "Intune".](https://docs.microsoft.com/intune/device-activation-lock-bypass)</span><span class="sxs-lookup"><span data-stu-id="ed6c6-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="ed6c6-112">**DUK**</span><span class="sxs-lookup"><span data-stu-id="ed6c6-112">**FAQ**</span></span>

<span data-ttu-id="ed6c6-113">Klausimas: **Aš išleido nuotolinio veiksmų pašalinti įmonės duomenis iš įrenginio, ir dabar jis įstrigo laukiančioje būsenoje.**</span><span class="sxs-lookup"><span data-stu-id="ed6c6-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="ed6c6-114">A: Kad nuotolinis veiksmas būtų sėkmingai užbaigtas, tikslinis įrenginys turi būti internete ir sveikas.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="ed6c6-115">Toliau nurodytais atvejais nuotolinis veiksmas lieka laukiančioje būsenoje 30 dienų arba tol, kol įrenginys patvirtina komandą, kai įrenginys:</span><span class="sxs-lookup"><span data-stu-id="ed6c6-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="ed6c6-116">Nėra ryšio.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-116">Does not have connectivity.</span></span>
- <span data-ttu-id="ed6c6-117">Praranda savo valdymo statusą su Intune.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="ed6c6-118">Jei manote, kad įrenginys nebeprisiregistruoja ir kad jis nepašalins įmonės duomenų, pasirinkite Naikinti.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="ed6c6-119">Panaikinus įrenginio įrašą pašalinamas, kad jis nebebūtų rodomas įrenginių sąraše Intune.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="ed6c6-120">Kad įrenginys vėl taptų aktyvus, jo vartotojas turi iš naujo užregistruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="ed6c6-121">Klausimas: **Kodėl tam tikrų nuotolinių veiksmų negalima naudoti?**</span><span class="sxs-lookup"><span data-stu-id="ed6c6-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="ed6c6-122">A: Ne visos platformos palaiko visus nuotolinio įrenginio veiksmus.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="ed6c6-123">Šie nuotoliniai veiksmai yra susiję su platforma.</span><span class="sxs-lookup"><span data-stu-id="ed6c6-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="ed6c6-124">Apeiti aktyvinimo užraktą (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="ed6c6-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="ed6c6-125">Nauja pradžia (tik "Windows")</span><span class="sxs-lookup"><span data-stu-id="ed6c6-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="ed6c6-126">Prarastas režimas (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="ed6c6-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="ed6c6-127">Įrenginio radimas (tik "iOS")</span><span class="sxs-lookup"><span data-stu-id="ed6c6-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="ed6c6-128">Paleisti iš naujo (tik "Windows")</span><span class="sxs-lookup"><span data-stu-id="ed6c6-128">Restart (Windows only)</span></span>

<span data-ttu-id="ed6c6-129">Daugiau informacijos apie kiekvieną veiksmą ieškokite [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="ed6c6-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>