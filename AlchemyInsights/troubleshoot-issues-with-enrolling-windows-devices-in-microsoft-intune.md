---
title: Trikčių šalinimas naudojant "Microsoft Intune" "Windows" įrenginius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708898"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Trikčių šalinimas naudojant "Microsoft Intune" "Windows" įrenginius

Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar.
  
Kai kurie dažniausi klaidų laiškai ir sprendimo būdai:
  
 **Programinės įrangos negalima įdiegti, 0x80cf4017:** Jūsų abonemento sertifikato galiojimas baigėsi. Iš naujo Atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje. Daugiau informacijos ieškokite šiame dokumentacijoje.
  
 **Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:
  
-  Vartotojas turi daugiau įrenginių, kuriuos užregistravote kaip įrenginio limitą. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Vartotojai gali prisijungti prie įrenginių į" Azure AD "nustatyta į" nėra ". Nustatykite visiems arba pasirinkite vartotojus. Daugiau informacijos ieškokite [šiame dokumentacijoje](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Įrenginį jau užregistravote kitas vartotojas. Jei taip, pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išregistruokite įrenginį prieš bandydami dar kartą.

-  Įrenginys yra "Windows 10 Home". Tik "Windows 10 Pro", "Education" ir "Enterprise SKU" gali prisijungti prie "Azure Active Directory".

Papildomi ištekliai, padėsiantys išspręsti problemą:
  
-  Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis. Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau.

-  Peržiūrėkite šiuos dokumentus, jei norite peržiūrėti dažnai pasitaikančių klaidų sąrašą, neleidžiančias įtraukti įtraukimo ir rezoliucijas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [diagnostikos dokumentas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune"](https://docs.microsoft.com/intune/windows-enroll).
