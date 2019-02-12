---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "Windows" įrenginiai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934784"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Šalinkite triktis naudodami werbowania į Microsoft Intune "Windows" įrenginiai

Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai. 
  
Kai kurių įprastinių klaidos prane imų ir sprendimo veiksmai:
  
 **Negali būti įdiegta programinė įranga, 0x80cf4017:** Jūsų paskyros sertifikatas nebegalioja. Iš naujo atsisiųsti PC kliento programinės įrangos paketą Intune administratoriaus konsolėje. Peržiūrėti šiuos dokumentus daugiau informacijos. 
  
 **Klaidos kodas 0x801c0003:** Klaida gali atsirasti šie scenarijai: 
  
1. Vartotojas turi daugiau įrenginius, užregistruotus nei įrenginio. Peržiūrėkite šiuos dokumentus [pašalinti įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeisti įrenginio](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Vartotojai gali prisijungti prie įrenginių Azure AD" nustatykite "none". Nustatyti visiems arba pasirinkite vartotojai. Peržiūrėkite [šiuos dokumentus](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) daugiau informacijos. 
    
3. Prietaisas jau mokosi kitas vartotojas. Jei tai byla, pašalinti įrenginį iš Azure Intune konsolės arba rankiniu būdu unenroll įrenginį, prieš bandydami dar kartą.
    
4. Prietaisas veikia Windows 10 namuose. Tik "Windows 10 Pro", švietimo ir Enterprise SKU prisijungti prie Azure Active Directory.
    
Papildomų išteklių, kurie padės išspręsti jūsų problemą:
  
1. Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių. Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Peržiūrėkite šiuos dokumentus bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą: [trikčių diagnostikos vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių diagnostika doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Sužinokite, kaip įtraukti į Microsoft Intune "Windows" įrenginiuose](https://docs.microsoft.com/intune/windows-enroll).
  

