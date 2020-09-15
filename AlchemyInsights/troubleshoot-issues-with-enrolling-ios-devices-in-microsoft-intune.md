---
title: Trikčių diagnostika naudojant "Microsoft Intune" "iOS" įrenginius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669256"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="a4d6d-102">Trikčių diagnostika naudojant "Microsoft Intune" "iOS" įrenginius</span><span class="sxs-lookup"><span data-stu-id="a4d6d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="a4d6d-103">Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="a4d6d-104">Kai kurie dažniausi klaidų laiškai ir sprendimo būdai:</span><span class="sxs-lookup"><span data-stu-id="a4d6d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="a4d6d-105">**Pasiektas įrenginio dangtelis** Vartotojas turi daugiau įrenginių, kuriuos užregistravote kaip įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a4d6d-106">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a4d6d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="a4d6d-107">**Ši tarnyba nepalaikoma. Registracijos strategijos nėra:** "Apple" "Push" pranešimų tarnyba (APNS) turi būti sukonfigūruota arba atnaujinta.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="a4d6d-108">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , kad sužinotumėte, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="a4d6d-109">**Vartotojo licencijos tipas neteisingas arba vartotojo vardas neatpažintas:** Vartotojui reikia priskirti Intune arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a4d6d-110">Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją naudodami: " [Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba " [Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="a4d6d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="a4d6d-111">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="a4d6d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a4d6d-112">Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a4d6d-113">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau.</span><span class="sxs-lookup"><span data-stu-id="a4d6d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="a4d6d-114">Peržiūrėkite šiuos dokumentus, jei norite peržiūrėti dažnai pasitaikančių klaidų sąrašą, neleidžiančias įtraukti įtraukimo ir rezoliucijas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a4d6d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="a4d6d-115">[Sužinokite, kaip užregistruoti "iOS" įrenginius "Microsoft Intune"](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="a4d6d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

