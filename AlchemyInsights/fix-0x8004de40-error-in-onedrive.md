---
title: Nustatyti 0x8004de40 klaida "OneDrive"
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133984"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Nustatyti 0x8004de40 klaida "OneDrive"

Jei gaunate klaidos 0x8004de40 naudojant "OneDrive":

- Iš naujo paleisti dėl nukentėjusių kompiuterio, prisijungę prie savo aktyvus Directory domeno.
- Jei iš naujo nėra išspręsti šią problemą, atsijungti ir prisijungti įrenginį iš Azure AD. 

**Pastaba**: turite būti įmonės tinklo atlikdami šiuos veiksmus. Nereikia atlikti šiuos veiksmus, kai jūs negalite prisijungti prie savo įmonės infrastruktūrą (pavyzdžiui, kelionės metu). 

- Atidarykite didesnių teisių komandų eilutę. 
- Atidarykite komandų eilutę, spustelėkite - **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**ir spustelėkite **paleisti kaip administratorius**.
- Įveskite *dsregcmd /leave* ir paspauskite **Enter**.
- Kai baigtas, įveskite *dsregcmd /join* ir paspauskite **Enter**.
- Kai baigtas, uždaryti į komandų eilutę.
- Iš naujo paleiskite kompiuterį ir prisijunkite prie "OneDrive".