---
title: Sąlyginė prieiga su "Intune"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069720"
---
# <a name="conditional-access-with-intune"></a>Sąlyginė prieiga su "Intune"

Naudojant  **sąlyginę prieigą**  su "Intune" reikia atlikti 3 veiksmus:

- Sukurkite **atitikties strategiją** (["Android",](https://docs.microsoft.com/intune/compliance-policy-create-android) ["iOS"](https://docs.microsoft.com/intune/compliance-policy-create-ios)Windows " ), kad apibrėžtumėte parametrus, kurie turi būti įvykdyti, kad įrenginys būtų laikomas atitinkančiu reikalavimus. [](https://docs.microsoft.com//intune/compliance-policy-create-windows) Pvz., įrenginys turi turėti bent 6 skaitmenų smeigtuką, kad jis būtų laikomas atitinkančiu reikalavimus.
- Sukurkite **sąlyginės prieigos strategiją,**  kuri apibrėžia, kokie ištekliai yra apsaugoti ir kokios sąlygos turi būti įvykdytos norint pasiekti šiuos išteklius.  [Pvz.,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  įrenginys turi atitikti reikalavimus prieš pasiekti įmonės el. paštą.
- Užtikrinti, **kad atitikties strategijos**  ir  **sąlyginės prieigos**  strategijos būtų nukreiptos į norimas vartotojų grupes. Tam gali reikėti sukurti konkrečias vartotojų grupes "Azure Active Directory".

**Naudingi saitai:**

[Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA trikčių diagnostika](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Trikčių diagnostikos strategija](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Norint apsaugoti el. Exchange (internetinę) nuo prieigos nekompiutentinguose įrenginiuose, turi būti laikomasi abiejų dokumentų:

1. [El. pašto prieigos apsauga nuo įrenginių naudojant EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [El. pašto prieigos apsauga nuo įrenginių naudojant modernius autentifikavimo klientus, pvz., Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)