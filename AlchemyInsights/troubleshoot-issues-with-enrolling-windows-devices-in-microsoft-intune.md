---
title: Šalinti triktis su mokosi Windows įrenginių Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665840"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Šalinti triktis su mokosi Windows įrenginių Microsoft Intune

Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.
  
Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:
  
 **Programinė įranga negali būti įdiegta, 0x80cf4017:** Jūsų paskyros sertifikato galiojimo laikas baigėsi. Iš naujo atsisiųsti PC kliento programinės įrangos paketą Intune administratoriaus konsolėje. Norėdami gauti daugiau informacijos, Peržiūrėkite šį dokumentą.
  
 **Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:
  
-  Vartotojas turi daugiau įrenginių įtraukti nei įrenginio limitą. Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Vartotojai gali prisijungti prie įrenginių Azure AD" nustatyta kaip "nė vienas." Nustatykite ją visiems arba pasirinkite vartotojus. Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Įrenginys jau yra užregistruotas kito vartotojo. Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išregistruokite įrenginį prieš bandydami dar kartą.

-  Įrenginys yra "Windows 10 Home". Tik Windows 10 Pro, švietimas ir Enterprise SKU gali prisijungti prie Azure Active Directory.

Papildomi ištekliai, padėsię išspręsti problemą.
  
-  Naudokite [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos triktis. Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) .

-  Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas bendrų klaidų, kurios neleidžia registracijos ir rezoliucijų, sąrašas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)".
