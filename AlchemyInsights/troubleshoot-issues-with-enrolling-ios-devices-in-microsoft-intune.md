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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Spręsti problemas, susijusias su mokosi ios įrenginių Microsoft Intune

Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar. 
  
Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:
  
- **Pasiekto įrenginio dangtelis** Vartotojas turi daugiau įrenginių įtraukti nei įrenginio limitą. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ši paslauga nepalaikoma. Nėra registracijos politika:** Apple Push pranešimų tarnyba (APNS) turi būti sukonfigūruotas arba atnaujintas. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ir vykdykite instrukcijas, kaip tai padaryti. 
    
- **Vartotojo licencijos tipas neteisingas arba vartotojo vardas neatpažintas:** Vartotojui reikia priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus, Norėdami priskirti licenciją per: " [Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba " [Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Papildomi ištekliai, padėsię išspręsti problemą.
  
1. Naudokite [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos triktis. Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas bendrų klaidų, kurios neleidžia registracijos ir rezoliucijų, sąrašas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Sužinokite, kaip registruotis iOS įrenginiai Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

