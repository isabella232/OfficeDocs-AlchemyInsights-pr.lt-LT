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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525067"
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