---
title: Trikčių šalinimas naudojant "Microsoft Intune" "Android" įrenginius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709006"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="54bbf-102">Trikčių šalinimas naudojant "Microsoft Intune" "Android" įrenginius</span><span class="sxs-lookup"><span data-stu-id="54bbf-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="54bbf-103">Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="54bbf-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="54bbf-104">Kai kurios Dažniausios problemos ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="54bbf-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="54bbf-105">**Įrenginio neužšifruota klaida įmonės portale:** Naujesnės "Android" versijos, ypač pradedant nuo v 7.0, reikalauja paleisties slaptojo kodo, kad įsitikintumėte, jog jūsų įrenginys visiškai šifruotas.</span><span class="sxs-lookup"><span data-stu-id="54bbf-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="54bbf-106">Įprasti sprendimai yra įgalinti paleisties PIN arba visiškai užšifruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="54bbf-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="54bbf-107">Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="54bbf-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="54bbf-108">**Įrenginių nepavyksta patikrinti naudojant Intune tarnybą arba Rodyti kaip "nesveika" Intune administravimo konsolėje:** Kai kurie "Samsung" 4,4 ir "5,5" įrenginiai gali netikrinti tarnybos.</span><span class="sxs-lookup"><span data-stu-id="54bbf-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="54bbf-109">Yra 3 galimi šios problemos sprendimo būdai:</span><span class="sxs-lookup"><span data-stu-id="54bbf-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="54bbf-110">Neautomatiškai atidarykite "Intune" įmonės portalo programą, kuri automatiškai pradės įrenginio sinchronizavimą.</span><span class="sxs-lookup"><span data-stu-id="54bbf-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="54bbf-111">Atnaujinkite įrenginį į "Android" 6,0 arba naujesnę versiją.</span><span class="sxs-lookup"><span data-stu-id="54bbf-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="54bbf-112">Išjunkite "Samsung Smart Manager" naudodami "Intune" įmonės portalą.</span><span class="sxs-lookup"><span data-stu-id="54bbf-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="54bbf-113">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , kad sužinotumėte daugiau apie šias problemas ir rezoliucijas.</span><span class="sxs-lookup"><span data-stu-id="54bbf-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="54bbf-114">**Vartotojo licencijos tipas neleistinas** arba **vartotojo vardas neatpažinta klaida:** vartotojui reikia priskirti Intune arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="54bbf-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="54bbf-115">Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją naudodami: "Office" administravimo centras arba "Azure" portalas.</span><span class="sxs-lookup"><span data-stu-id="54bbf-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="54bbf-116">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="54bbf-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="54bbf-117">Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="54bbf-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="54bbf-118">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau.</span><span class="sxs-lookup"><span data-stu-id="54bbf-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="54bbf-119">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) , kad būtų dažnai pasitaikančių klaidų, neleidžiančių atlikti įtraukimo ir sprendimų, sąrašas.</span><span class="sxs-lookup"><span data-stu-id="54bbf-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="54bbf-120">[Sužinokite, kaip užregistruoti "Android" įrenginius programoje "Microsoft Intune"](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="54bbf-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
