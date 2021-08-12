---
title: Gedimų "OneDrive" trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921015"
---
# <a name="troubleshoot-onedrive-crashes"></a>Gedimų "OneDrive" trikčių šalinimas

Jei "OneDrive" kelis kartus sugenda, pabandykite atlikti šiuos trikčių šalinimo veiksmus:

**Įsitikinkite, kad registro raktai nėra nustatyti:**

1. Naudodami registro rengyklę eikite į HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jei Yra DisableFileSyncNGSC ir nustatyta kaip 1, atidarykite raktą ir pakeiskite reikšmę į 0.
3. Rankiniu būdu paleiskite "OneDrive" nueikite į Pradžia ![Paspauskite Windows klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)įveskite "OneDrive" ieškos lauke, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

**Iš naujo "OneDrive":**

Pastabos:

- Iš naujo nustačius "OneDrive" bus atjungti visi esami sinchronizavimo ryšiai (įskaitant asmeninę "OneDrive", jei nustatyta).
- Neprarasite failų ar duomenų iš naujo nustatydami "OneDrive" kompiuteryje.

**Norėdami iš naujo "OneDrive":**

1. Atidarykite dialogo langą Vykdyti paspausdami klavišą Windows R.
2. Įveskite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ir paspauskite Gerai. Komandos langas gali būti rodomas trumpai.
3. Rankiniu būdu paleiskite "OneDrive" nueikite į Pradžia ![Paspauskite Windows klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)įveskite "OneDrive" ieškos lauke, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

Pastabos:

- Jei prieš iš naujo nustatę sinchronizavimą pasirinkote sinchronizuoti tik kai kuriuos aplankus, turėsite tai padaryti dar kartą, kai bus baigtas sinchronizavimas. Daugiau [informacijos rasite "OneDrive" aplankų, kuriuos norite sinchronizuoti su kompiuteriu,](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pasirinkimas.
- Turėsite tai atlikti savo asmeniniams "OneDrive" ir "OneDrive" verslui.