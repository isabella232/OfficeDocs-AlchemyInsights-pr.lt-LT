---
title: "\"Android\" įrenginių registracijos \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830950"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="07f41-102">"Android" įrenginių registracijos "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="07f41-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="07f41-103">Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="07f41-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="07f41-104">Kai kurios dažniausios problemos ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="07f41-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="07f41-105">**Įrenginio nešifruota klaida įmonės portale:** Naujesnėms "Android" versijoms, ypač pradedant nuo v7.0, reikalingas paleisties slaptasis kodas, kad įsitikintumėte, jog jūsų įrenginys visiškai užšifruotas.</span><span class="sxs-lookup"><span data-stu-id="07f41-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="07f41-106">Bendrieji sprendimai yra įjungti paleisties smeigtuką arba visiškai šifruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="07f41-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="07f41-107">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="07f41-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="07f41-108">**Įrenginiams nepavyksta prisijungti naudojant "Intune" tarnybą arba "Intune" administravimo konsolėje rodyti kaip "Nesveika":** Kai kurie "Samsung 4.4" ir "5.5" įrenginiai gali nepatikrinti paslaugos.</span><span class="sxs-lookup"><span data-stu-id="07f41-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="07f41-109">Yra 3 galimi šios problemos sprendimai:</span><span class="sxs-lookup"><span data-stu-id="07f41-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="07f41-110">Rankiniu būdu atidarykite "Intune" įmonės portalo programą, kuri automatiškai inicijuoja įrenginio sinchronizavimą.</span><span class="sxs-lookup"><span data-stu-id="07f41-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="07f41-111">Atnaujinkite įrenginį į "Android 6.0" arba naujesnė versija.</span><span class="sxs-lookup"><span data-stu-id="07f41-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="07f41-112">Išjunkite "Samsung Smart Manager" nuo "Intune" įmonės portalo valdymo.</span><span class="sxs-lookup"><span data-stu-id="07f41-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="07f41-113">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) jei reikia daugiau informacijos apie šias problemas ir sprendimą.</span><span class="sxs-lookup"><span data-stu-id="07f41-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="07f41-114">**Klaida Vartotojo licencijos tipas** **netinkamas arba Vartotojo** vardas neatpažintas: vartotojui turi būti priskirta "Intune" arba EMS licencija.</span><span class="sxs-lookup"><span data-stu-id="07f41-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="07f41-115">Peržiūrėkite šiuos dokumentus ir priskirkite licenciją per: "Office" administravimo centrą arba "Azure" portalą.</span><span class="sxs-lookup"><span data-stu-id="07f41-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="07f41-116">Papildomi ištekliai, kurie padės išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="07f41-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="07f41-117">Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="07f41-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="07f41-118">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="07f41-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="07f41-119">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) kad peržiūrėtumėte dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieną iš jų, sąrašą.</span><span class="sxs-lookup"><span data-stu-id="07f41-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="07f41-120">[Sužinokite, kaip užregistruoti "Android" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="07f41-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
