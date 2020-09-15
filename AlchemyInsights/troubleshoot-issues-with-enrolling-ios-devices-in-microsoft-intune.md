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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Trikčių diagnostika naudojant "Microsoft Intune" "iOS" įrenginius

Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar. 
  
Kai kurie dažniausi klaidų laiškai ir sprendimo būdai:
  
- **Pasiektas įrenginio dangtelis** Vartotojas turi daugiau įrenginių, kuriuos užregistravote kaip įrenginio limitą. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ši tarnyba nepalaikoma. Registracijos strategijos nėra:** "Apple" "Push" pranešimų tarnyba (APNS) turi būti sukonfigūruota arba atnaujinta. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , kad sužinotumėte, kaip tai padaryti. 
    
- **Vartotojo licencijos tipas neteisingas arba vartotojo vardas neatpažintas:** Vartotojui reikia priskirti Intune arba EMS licenciją. Peržiūrėkite šiuos dokumentus, kad priskirtumėte licenciją naudodami: " [Office" administravimo centras](https://docs.microsoft.com/intune/licenses-assign) arba " [Azure" portalas](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Papildomi ištekliai, padėsiantys išspręsti problemą:
  
1. Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau. 
    
2. Peržiūrėkite šiuos dokumentus, jei norite peržiūrėti dažnai pasitaikančių klaidų sąrašą, neleidžiančias įtraukti įtraukimo ir rezoliucijas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) ir [diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Sužinokite, kaip užregistruoti "iOS" įrenginius "Microsoft Intune"](https://docs.microsoft.com/intune/ios-enroll).
    

