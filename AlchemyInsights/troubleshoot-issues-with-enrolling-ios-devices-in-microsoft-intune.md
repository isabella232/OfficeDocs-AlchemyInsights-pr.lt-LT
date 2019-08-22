---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "iOS" įrenginiai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507011"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b3964-102">Šalinkite triktis naudodami werbowania į Microsoft Intune "iOS" įrenginiai</span><span class="sxs-lookup"><span data-stu-id="b3964-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b3964-103">Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai.</span><span class="sxs-lookup"><span data-stu-id="b3964-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b3964-104">Kai kurių įprastinių klaidos prane imų ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="b3964-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b3964-105">**Įrenginio dangtelį, pasiekė** Vartotojas turi daugiau įrenginius, užregistruotus nei įrenginio.</span><span class="sxs-lookup"><span data-stu-id="b3964-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="b3964-106">Peržiūrėkite šiuos dokumentus [pašalinti įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeisti įrenginio](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b3964-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b3964-107">**Ši paslauga nėra palaikomas. Jokių registracijos politiką:** Apple Push pranešimų paslauga (APN) turi būti sukonfigūruotas arba atnaujintos.</span><span class="sxs-lookup"><span data-stu-id="b3964-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="b3964-108">Peržiūrėti [šiame dokumente](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) nurodymų, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="b3964-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b3964-109">**Vartotojo licencijos tipas neleistinas arba neatpažįstamas vartotojo vardas:** Vartotojas turi priskirti Intune arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="b3964-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b3964-110">Peržiūrėkite šiuos dokumentus priskirti licenciją per: [Office administravimo centro](https://docs.microsoft.com/intune/licenses-assign) arba [Azure portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="b3964-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b3964-111">Papildomų išteklių, kurie padės išspręsti jūsų problemą:</span><span class="sxs-lookup"><span data-stu-id="b3964-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b3964-112">Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių.</span><span class="sxs-lookup"><span data-stu-id="b3964-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b3964-113">Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="b3964-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b3964-114">Peržiūrėkite šiuos dokumentus bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą: [trikčių diagnostikos vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių diagnostika doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b3964-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b3964-115">[Sužinokite, kaip registruotis į Microsoft Intune "iOS" įrenginiai](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="b3964-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

