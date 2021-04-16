---
title: "\"Windows\" įrenginių registracijos \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808979"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>"Windows" įrenginių registracijos "Microsoft Intune" trikčių šalinimas

Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.
  
Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:
  
 **Programinės įrangos įdiegti negalima, 0x80cf4017:** Jūsų paskyros sertifikato galiojimo laikas baigėsi. Iš naujo atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje. Peržiūrėkite šią dokumentaciją, jei reikia daugiau informacijos.
  
 **Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:
  
-  Vartotojas turi daugiau įrenginių, užregistruotų už įrenginio limitą. Peržiūrėkite šiuos [dokumentus, kad pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) [arba pakeistumėte įrenginio limitą.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Vartotojai gali prisijungti prie įrenginių prie "Azure AD", nustatyta kaip "nėra". Nustatykite jį visiems arba pasirinkite vartotojus. Peržiūrėkite [šią dokumentaciją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) jei reikia daugiau informacijos.

-  Įrenginį jau užregistravo kitas vartotojas. Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu atjunkite įrenginį prieš bandydami dar kartą.

-  Įrenginys yra "Windows 10 Home". Prie "Azure Active Directory" gali prisijungti tik "Windows 10 Pro", "Education" ir "Enterprise" SKU.

Papildomi ištekliai, kurie padės išspręsti problemą:
  
-  Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.

-  Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas sąrašas dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieno iš jų: Trikčių diagnostikos [vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ir Trikčių diagnostikos dokumentas.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Sužinokite, kaip registruoti "Windows" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/windows-enroll)
