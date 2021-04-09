---
title: "\"OneDrive 0x8004de40 klaidos taisymas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649756"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>"OneDrive 0x8004de40 klaidos taisymas

Jei naudojate "Windows 7" ir gaunate šią klaidą, naujinimas, kad [įgalintumėte TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" sistemoje "Windows".](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jei naudojate "Windows 10" ir gaunate klaidos 0x8004de40 "OneDrive":

- Perkraukite paveiktą kompiuterį, kai esate prisijungę prie "Acitve Directory" domeno.
- Jei paleidimas iš naujo problemos neišspręs, atjunkite ir vėl prijunkite įrenginį iš "Azure AD". 

**Pastaba:** atlikdami šiuos veiksmus turėtumėte būti įmonės tinkle. Neatlikite šių veiksmų, kai nesate prisijungę prie įmonės infrastruktūros (pvz., keliaudami). 

1. Atidarykite didesnių teisių komandinę eilutę **pasirinkdami Pradžia**, dešiniuoju pelės mygtuku spustelėkite **Komandinė** eilutė , tada pasirinkite **Vykdyti administratoriaus teisėmis**.

1. Įveskite *dsregcmd /leave ir* paspauskite **"Enter".**

1. Baigę įveskite *dsregcmd /join ir* paspauskite **"Enter".**

1. Baigę uždarykite komandinę eilutę.

1. Iš naujo paleiskite kompiuterį ir prisijunkite prie "OneDrive".