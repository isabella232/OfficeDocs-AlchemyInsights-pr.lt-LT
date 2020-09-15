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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658886"
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

-  Peržiūrėkite šiuos dokumentus, jei norite peržiūrėti dažnai pasitaikančių klaidų sąrašą, neleidžiančias įtraukti įtraukimo ir rezoliucijas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune"](https://docs.microsoft.com/intune/windows-enroll).
