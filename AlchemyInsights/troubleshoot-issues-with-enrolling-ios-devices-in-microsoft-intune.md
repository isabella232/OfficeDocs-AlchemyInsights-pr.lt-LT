---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "iOS" įrenginiai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480917"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e0239-102">Šalinkite triktis naudodami werbowania į Microsoft Intune "iOS" įrenginiai</span><span class="sxs-lookup"><span data-stu-id="e0239-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e0239-103">Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai.</span><span class="sxs-lookup"><span data-stu-id="e0239-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e0239-104">Kai kurių įprastinių klaidos prane imų ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="e0239-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e0239-p101">**Įrenginio dangtelį, pasiekė** Vartotojas turi daugiau įrenginius, užregistruotus nei įrenginio. Peržiūrėkite šiuos dokumentus [pašalinti įrenginį](https://docs.microsoft.com/en-us/intune/devices-wipe) arba [pakeisti įrenginio](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e0239-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e0239-p102">**Ši paslauga nėra palaikomas. Jokių registracijos politiką:** Apple Push pranešimų paslauga (APN) turi būti sukonfigūruotas arba atnaujintos. Peržiūrėti [šiame dokumente](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) nurodymų, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="e0239-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e0239-p103">**Vartotojo licencijos tipas neleistinas arba neatpažįstamas vartotojo vardas:** Vartotojas turi priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus priskirti licenciją per: [Office administravimo centro](https://docs.microsoft.com/en-us/intune/licenses-assign) arba [Azure portalas](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="e0239-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e0239-111">Papildomų išteklių, kurie padės išspręsti jūsų problemą:</span><span class="sxs-lookup"><span data-stu-id="e0239-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e0239-p104">Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių. Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/en-us/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="e0239-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e0239-114">Peržiūrėkite šiuos dokumentus bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą: [trikčių diagnostikos vadovas](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių diagnostika doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e0239-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e0239-115">[Sužinokite, kaip registruotis į Microsoft Intune "iOS" įrenginiai](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="e0239-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

