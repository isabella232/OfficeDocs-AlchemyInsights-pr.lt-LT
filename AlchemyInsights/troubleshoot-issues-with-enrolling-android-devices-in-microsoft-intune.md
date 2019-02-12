---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "Android" įrenginių
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939356"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="2dae2-102">Šalinkite triktis naudodami werbowania į Microsoft Intune "Android" įrenginių</span><span class="sxs-lookup"><span data-stu-id="2dae2-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="2dae2-103">Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai.</span><span class="sxs-lookup"><span data-stu-id="2dae2-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2dae2-104">Kai kurios Dažnos problemos ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="2dae2-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="2dae2-p101">**Prietaisas nėra šifruojami klaida įmonės portale:** Naujesnių versijų "Android", ypač pradedant v7.0, reikalauja paleisties kodą, norėdami įsitikinti, kad jūsų įrenginys yra visiškai iššifruoti. Bendri sprendimai yra įgalinti paleisties pin arba visiškai šifruoti prietaiso. Peržiūrėti [šio dokumento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dėl daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="2dae2-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="2dae2-p102">**Įrenginių nesugeba patikrinti su Intune tarnyba arba Rodyti kaip "Nesveiko" Intune administratoriaus konsolėje:** Kai kurios "Samsung" 4.4 ir 5.5 įrenginiai negali tikrinti ir eksploatuoti. Yra 3 galimi siekiant šią problemą:</span><span class="sxs-lookup"><span data-stu-id="2dae2-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="2dae2-110">Rankiniu būdu atidaryti Intune įmonės portalo programą, kuri bus automatiškai pradėti įrenginio sinchronizavimą.</span><span class="sxs-lookup"><span data-stu-id="2dae2-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="2dae2-111">Atnaujinti įrenginio į "Android" 6.0 arba naujesnė.</span><span class="sxs-lookup"><span data-stu-id="2dae2-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="2dae2-p103">Išjungti Samsung Smart Manager valdymo Intune įmonės portalas. Peržiūrėti daugiau informacijos apie šios problemos ir sprendimai [šiame dokumente](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .</span><span class="sxs-lookup"><span data-stu-id="2dae2-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="2dae2-p104">**Vartotojo licencijos tipas neteisingas** arba **vartotojo vardas nėra atpažįstamas klaida:** vartotojas turi priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus priskirti licenciją per: Office administravimo centro arba Azure portalas.</span><span class="sxs-lookup"><span data-stu-id="2dae2-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="2dae2-116">Papildomų išteklių, kurie padės išspręsti jūsų problemą:</span><span class="sxs-lookup"><span data-stu-id="2dae2-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2dae2-p105">Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių. Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="2dae2-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2dae2-119">Peržiūrėti [šį dokumentą](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą.</span><span class="sxs-lookup"><span data-stu-id="2dae2-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="2dae2-120">[Sužinokite, kaip Registruotis "Android" įrenginius į Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="2dae2-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

