---
title: "\"iOS\" įrenginių registracijos \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823471"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="07bf6-102">"iOS" įrenginių registracijos "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="07bf6-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="07bf6-103">Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="07bf6-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="07bf6-104">Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="07bf6-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="07bf6-105">**Pasiektas įrenginio dangtelis** Vartotojas turi daugiau įrenginių, užregistruotų už įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="07bf6-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="07bf6-106">Peržiūrėkite šiuos [dokumentus, kad pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) [arba pakeistumėte įrenginio limitą.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="07bf6-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="07bf6-107">**Ši tarnyba nepalaikoma. Nėra registracijos strategijos: "Apple** Push" pranešimų tarnyba (APNS) turi būti sukonfigūruota arba atnaujinta.</span><span class="sxs-lookup"><span data-stu-id="07bf6-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="07bf6-108">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) jei reikia instrukcijų, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="07bf6-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="07bf6-109">**Vartotojo licencijos tipas netinkamas arba vartotojo vardas neatpažintas:** Vartotojui turi būti priskirta "Intune" arba EMS licencija.</span><span class="sxs-lookup"><span data-stu-id="07bf6-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="07bf6-110">Peržiūrėkite šiuos dokumentus ir priskirkite licenciją per: ["Office" administravimo centras arba](https://docs.microsoft.com/intune/licenses-assign) ["Azure" portalas.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="07bf6-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="07bf6-111">Papildomi ištekliai, kurie padės išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="07bf6-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="07bf6-112">Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="07bf6-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="07bf6-113">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="07bf6-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="07bf6-114">Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas sąrašas dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieno iš jų: Trikčių diagnostikos [vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ir Trikčių diagnostikos dokumentas.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="07bf6-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="07bf6-115">[Sužinokite, kaip užregistruoti "iOS" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="07bf6-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

