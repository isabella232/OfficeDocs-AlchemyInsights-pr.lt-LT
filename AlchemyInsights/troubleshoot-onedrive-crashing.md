---
title: "\"OneDrive\" gedimų šalinimas"
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826207"
---
# <a name="troubleshoot-onedrive-crashes"></a>"OneDrive" gedimų šalinimas

Jei "OneDrive" kelis kartus sugenda, pabandykite atlikti šiuos trikčių šalinimo veiksmus:

**Įsitikinkite, kad registro raktai nėra nustatyti:**

1. Naudodami registro rengyklę eikite į HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jei Yra DisableFileSyncNGSC ir nustatyta kaip 1, atidarykite raktą ir pakeiskite reikšmę į 0.
3. Rankiniu būdu paleiskite "OneDrive" nueidami į Pradžia ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite OneDrive, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

**"OneDrive" nustatymas iš naujo:**

Pastabos:

- Iš naujo nustačius "OneDrive", atjungiami visi esami sinchronizavimo ryšiai (įskaitant asmeninę "OneDrive", jei nustatyta).
- Iš naujo nustatydami "OneDrive" kompiuteryje neprarasite failų ar duomenų.

**Norėdami iš naujo nustatyti "OneDrive":**

1. Atidarykite dialogo langą Vykdyti paspausdami "Windows" klavišą ir R.
2. Įveskite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ir paspauskite Gerai. Komandos langas gali būti rodomas trumpai.
3. Rankiniu būdu paleiskite "OneDrive" nueidami į Pradžia ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite OneDrive, tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

Pastabos:

- Jei prieš iš naujo nustatę sinchronizavimą pasirinkote sinchronizuoti tik kai kuriuos aplankus, turėsite tai padaryti dar kartą, kai bus baigtas sinchronizavimas. Norėdami [gauti daugiau informacijos, skaitykite Pasirinkite, kuriuos "OneDrive" aplankus](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)sinchronizuoti su jūsų   kompiuteriu.
- Turėsite tai atlikti asmeninėje "OneDrive" ir "OneDrive" verslui.