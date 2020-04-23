---
title: "\"iOS\" įrenginių įtraukimo į \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736166"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="3918e-102">"iOS" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="3918e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="3918e-103">Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="3918e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="3918e-104">Kai kurie dažniausiai pasitaikantys klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="3918e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="3918e-105">**Pasiektas įrenginio dangtelis** Vartotojas turi daugiau įrenginių, įtrauktų nei įrenginio riba.</span><span class="sxs-lookup"><span data-stu-id="3918e-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3918e-106">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3918e-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="3918e-107">**Ši tarnyba nepalaikoma. Nėra registracijos strategijos:** "Apple Push" pranešimų tarnyba (APNS) turi būti sukonfigūruota arba atnaujinta.</span><span class="sxs-lookup"><span data-stu-id="3918e-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="3918e-108">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) jei reikia instrukcijų, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="3918e-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="3918e-109">**Vartotojo licencijos tipas neleistinas arba vartotojo vardas neatpažįstamas:** Vartotojui turi būti priskirta "Intune" arba EMS licencija.</span><span class="sxs-lookup"><span data-stu-id="3918e-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3918e-110">Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją per: ["Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba ["Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="3918e-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="3918e-111">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="3918e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3918e-112">Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas.</span><span class="sxs-lookup"><span data-stu-id="3918e-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3918e-113">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="3918e-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="3918e-114">Peržiūrėkite šiuos dokumentus, kad būtų pateiktas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir šalinti kiekvieno sąskirstys: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių šalinimo dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune), sąrašas.</span><span class="sxs-lookup"><span data-stu-id="3918e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="3918e-115">[Sužinokite, kaip registruoti "iOS" įrenginius programoje "Microsoft Intune".](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="3918e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

