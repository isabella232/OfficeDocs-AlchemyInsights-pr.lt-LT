---
title: Prisijungimo prie "Microsoft 365" programėlių problemos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579945"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>"Microsoft 365" programėlių taisymas "Atsiprašome, jau prisijungęs kitas jūsų organizacijos abonementas"

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Pašalinkite visus darbo abonementus, išskyrus paveiktą abonementą, naudodami "Windows" parametrus > **"Access" darbą arba mokyklą**.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0. (Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidarykite "Office" programą, pasirinkite **Atsijungti prie**  >  **failų abonemento**  >  **Sign Out**. Tada prisijunkite naudodami vartotojo abonementą su galiojančia licencija. Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daugiau informacijos [ieškokite "Atsiprašome, kitas jūsų organizacijos abonementas jau prisijungęs šiame kompiuteryje" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).