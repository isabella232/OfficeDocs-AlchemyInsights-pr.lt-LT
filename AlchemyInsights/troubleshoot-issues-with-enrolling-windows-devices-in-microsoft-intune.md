---
title: "\"Windows\" įrenginių įtraukimo į \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665840"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>"Windows" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas

Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.
  
Kai kurie dažniausiai pasitaikantys klaidų pranešimai ir sprendimo veiksmai:
  
 **Programinės įrangos įdiegti negalima, 0x80cf4017:** Baigėsi abonemento sertifikato galiojimo laikas. Iš naujo atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje. Peržiūrėkite šią dokumentaciją, jei norite gauti daugiau informacijos.
  
 **Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:
  
-  Vartotojas turi daugiau įrenginių, įtrauktų nei įrenginio riba. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Vartotojai gali prisijungti prie įrenginių Azure AD" yra nustatyta kaip "nėra." Nustatykite jį visiems arba pasirinkite vartotojus. Peržiūrėkite [šią dokumentaciją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) jei norite gauti daugiau informacijos.

-  Įrenginį jau užregistravo kitas vartotojas. Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išnaujoužkite įrenginį prieš bandydami dar kartą.

-  Įrenginys yra "Windows 10 Home". Tik "Windows 10 Pro", "Education" ir "Enterprise" SKU gali prisijungti prie "Azure Active Directory".

Papildomi ištekliai, padėsiantys išspręsti problemą:
  
-  Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas. Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos.

-  Peržiūrėkite šiuos dokumentus, kad būtų pateiktas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir šalinti kiekvieno sąskirstys: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių šalinimo dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune), sąrašas.

[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/windows-enroll)
