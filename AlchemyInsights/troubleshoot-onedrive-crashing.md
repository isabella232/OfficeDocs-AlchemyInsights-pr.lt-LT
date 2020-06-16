---
title: "\"OneDrive\" gedimų trikčių diagnostika"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749162"
---
# <a name="troubleshoot-onedrive-crashes"></a>"OneDrive" gedimų trikčių diagnostika

Jei "OneDrive" kelis kartus užstringa, pabandykite atlikti šiuos trikčių šalinimo veiksmus:

**Įsitikinkite, kad registro raktai nenustatti:**

1. Naudodami registro rengyklę, eikite į HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jei DisableFileSyncNGSC yra ir nustatyta kaip 1, atidarykite raktą ir pakeiskite reikšmę į 0.
3. Rankiniu būdu paleiskite "OneDrive" nuėję į pradžios ekraną ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" darbalaukio programėlę.

**Iš naujo nustatyti "OneDrive":**

Pastabos:

- Iš naujo nustačius "OneDrive" atjungimi visi esami sinchronizavimo ryšiai (įskaitant asmeninį "OneDrive", jei nustatyta).
- Nenusirausdami failų ar duomenų iš naujo nustatydami "OneDrive" kompiuteryje.

**Norėdami iš naujo nustatyti "OneDrive":**

1. Atidarykite dialogo langą Vykdyti paspausdami "Windows" klavišą ir R.
2. Įveskite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ir paspauskite Gerai. Komandų langas gali pasirodyti trumpai.
3. Rankiniu būdu paleiskite "OneDrive" nuėję į pradžios ekraną ![Paspauskite "Windows" klavišą](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), ieškos lauke įveskite "OneDrive", tada spustelėkite "OneDrive" darbalaukio programėlę.

Pastabos:

- Jei pasirinkote sinchronizuoti tik kai kuriuos aplankus prieš nustatymą iš naujo, turėsite tai padaryti dar kartą, kai sinchronizavimas bus baigtas. Skaitykite Norėdami gauti daugiau informacijos, skaitykite [Pasirinkite, kuriuos "OneDrive" aplankus sinchronizuoti su kompiuteriu.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  
- Tai turėsite atlikti asmeniniam "OneDrive" ir "OneDrive" verslui.