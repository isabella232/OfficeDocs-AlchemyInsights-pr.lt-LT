---
title: Prisijungimo prie "Microsoft 365" programų problemos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695331"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>"Microsoft" 365 taikomųjų programų taisymas "Atsiprašome, kita jūsų organizacijos paskyra jau pasirašyta" pranešime

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą, naudodami "Windows" parametrus > " **Access" darbo arba mokymo įstaigos**.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į "16,0". (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidarykite "Office" programą, pasirinkite **failo**  >  **abonementas**  >  **Atsijungti**. Tada prisijunkite naudodami vartotojo paskyrą su galiojančia licencija. Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daugiau informacijos ieškokite " [Atsiprašome, kita jūsų organizacijos paskyra jau Prisijungta šiame kompiuteryje" Office "](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).