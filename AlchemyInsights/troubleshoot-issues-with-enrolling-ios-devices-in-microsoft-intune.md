---
title: Spręsti problemas, susijusias su mokosi ios įrenginių Microsoft Intune
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507011"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="69bb8-102">Spręsti problemas, susijusias su mokosi ios įrenginių Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="69bb8-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="69bb8-103">Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="69bb8-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="69bb8-104">Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="69bb8-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="69bb8-105">**Pasiekto įrenginio dangtelis** Vartotojas turi daugiau įrenginių įtraukti nei įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="69bb8-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="69bb8-106">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="69bb8-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="69bb8-107">**Ši paslauga nepalaikoma. Nėra registracijos politika:** Apple Push pranešimų tarnyba (APNS) turi būti sukonfigūruotas arba atnaujintas.</span><span class="sxs-lookup"><span data-stu-id="69bb8-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="69bb8-108">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ir vykdykite instrukcijas, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="69bb8-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="69bb8-109">**Vartotojo licencijos tipas neteisingas arba vartotojo vardas neatpažintas:** Vartotojui reikia priskirti Intune arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="69bb8-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="69bb8-110">Peržiūrėkite šiuos dokumentus, Norėdami priskirti licenciją per: " [Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba " [Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="69bb8-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="69bb8-111">Papildomi ištekliai, padėsię išspręsti problemą.</span><span class="sxs-lookup"><span data-stu-id="69bb8-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="69bb8-112">Naudokite [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="69bb8-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="69bb8-113">Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="69bb8-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="69bb8-114">Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas bendrų klaidų, kurios neleidžia registracijos ir rezoliucijų, sąrašas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="69bb8-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="69bb8-115">[Sužinokite, kaip registruotis iOS įrenginiai Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="69bb8-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

