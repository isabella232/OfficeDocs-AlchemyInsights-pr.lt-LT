---
title: "\"Android\" įrenginių įtraukimo į \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759628"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6c159-102">"Android" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="6c159-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6c159-103">Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="6c159-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6c159-104">Kai kurios dažniausios problemos ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="6c159-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6c159-105">**Įrenginio neužšifruota klaida įmonės portale:** Naujesnėms "Android" versijoms, ypač pradedant v7.0, reikia paleisties kodą, kad įsitikintumėte, jog jūsų įrenginys yra visiškai užšifruotas.</span><span class="sxs-lookup"><span data-stu-id="6c159-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="6c159-106">Įprasti sprendimai yra įgalinti paleisties smeigtuką arba visiškai užšifruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="6c159-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="6c159-107">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="6c159-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="6c159-108">**Įrenginiai nepavyksta patikrinti su Intune paslauga arba rodyti kaip "Nesveika" Intune administratoriaus konsolėje:** Kai kurie "Samsung 4.4" ir "5.5" įrenginiai gali netikrinti paslaugos.</span><span class="sxs-lookup"><span data-stu-id="6c159-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="6c159-109">Yra 3 galimi šios problemos sprendimai:</span><span class="sxs-lookup"><span data-stu-id="6c159-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="6c159-110">Rankiniu būdu atidarykite "Intune" įmonės portalo programą, kuri automatiškai pradės įrenginio sinchronizavimą.</span><span class="sxs-lookup"><span data-stu-id="6c159-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="6c159-111">Atnaujinkite įrenginį į 6.0 ar naujesnę "Android".</span><span class="sxs-lookup"><span data-stu-id="6c159-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="6c159-112">Išjunkite "Samsung Smart Manager" nuo "Intune" įmonės portalo valdymo.</span><span class="sxs-lookup"><span data-stu-id="6c159-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="6c159-113">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) jei reikia daugiau informacijos šiais klausimais ir sprendimais.</span><span class="sxs-lookup"><span data-stu-id="6c159-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="6c159-114">**Vartotojo licencijos tipas neleistinas** arba **vartotojo vardas neatpažintas klaida:** vartotojui reikia priskirti Intune arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="6c159-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6c159-115">Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją per: "Office" administravimo centras arba "Azure" portalas.</span><span class="sxs-lookup"><span data-stu-id="6c159-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="6c159-116">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="6c159-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6c159-117">Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas.</span><span class="sxs-lookup"><span data-stu-id="6c159-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6c159-118">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="6c159-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="6c159-119">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) kuriame pateikiamas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir priimti sprendimai kiekvienam, sąrašas.</span><span class="sxs-lookup"><span data-stu-id="6c159-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="6c159-120">[Sužinokite, kaip užregistruoti "Android" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="6c159-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
