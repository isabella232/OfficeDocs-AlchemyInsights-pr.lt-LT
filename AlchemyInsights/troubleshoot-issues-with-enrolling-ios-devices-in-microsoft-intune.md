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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>"iOS" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas

Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar. 
  
Kai kurie dažniausiai pasitaikantys klaidų pranešimai ir sprendimo veiksmai:
  
- **Pasiektas įrenginio dangtelis** Vartotojas turi daugiau įrenginių, įtrauktų nei įrenginio riba. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ši tarnyba nepalaikoma. Nėra registracijos strategijos:** "Apple Push" pranešimų tarnyba (APNS) turi būti sukonfigūruota arba atnaujinta. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) jei reikia instrukcijų, kaip tai padaryti. 
    
- **Vartotojo licencijos tipas neleistinas arba vartotojo vardas neatpažįstamas:** Vartotojui turi būti priskirta "Intune" arba EMS licencija. Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją per: ["Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba ["Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Papildomi ištekliai, padėsiantys išspręsti problemą:
  
1. Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos. 
    
2. Peržiūrėkite šiuos dokumentus, kad būtų pateiktas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir šalinti kiekvieno sąskirstys: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [trikčių šalinimo dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune), sąrašas.
    
3. [Sužinokite, kaip registruoti "iOS" įrenginius programoje "Microsoft Intune".](https://docs.microsoft.com/intune/ios-enroll)
    

