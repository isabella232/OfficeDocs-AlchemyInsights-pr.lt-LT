---
title: "\"OneDrive\" gedimų šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665006"
---
# <a name="troubleshoot-onedrive-crashes"></a>"OneDrive" gedimų šalinimas

Jei "OneDrive" kelis kartus sugenda, išbandykite šiuos trikčių šalinimo veiksmus:

**Įsitikinkite, kad registro raktų nėra nustatyta:**

1. Naudodami registro rengyklę eikite į HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Jei yra "Disablefilesyncntgs" ir nustatote 1, atidarykite raktą ir pakeiskite reikšmę į 0.
3. Neautomatiškai paleiskite "OneDrive" nuėję į pradžios ekraną ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

**Iš naujo nustatyti "OneDrive":**

Pastabų

- Iš naujo nustačius "OneDrive", Atjungiami visi esami sinchronizavimo ryšiai (įskaitant asmeninę "OneDrive", jei nustatyta).
- Neprarasite failų arba duomenų iš naujo nustatydami "OneDrive" savo kompiuteryje.

**Norėdami iš naujo nustatyti "OneDrive":**

1. Atidarykite dialogo langą vykdyti paspausdami "Windows" klavišą ir R.
2. Įveskite% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset ir paspauskite Gerai. Gali būti trumpai rodomas komandos langas.
3. Neautomatiškai paleiskite "OneDrive" nuėję į pradžios ekraną ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" kompiuterio taikomąją programą.

Pastabų

- Jei pasirinkote sinchronizuoti tik kai kuriuos aplankus prieš iš naujo, turėsite tai padaryti dar kartą baigus sinchronizuoti. Norėdami gauti daugiau informacijos, skaitykite [pasirinkite, kuriuos "OneDrive" aplankus sinchronizuoti su savo kompiuteriu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Turėsite tai atlikti asmeniniams "OneDrive" ir "OneDrive" verslui.