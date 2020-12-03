---
title: Įgalinkite slaptažodžio atgalinį įrašymą „Azure AD Connect“
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
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560448"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Įgalinkite slaptažodžio atgalinį įrašymą „Azure AD Connect“

Jei norite įjungti savitarnos slaptažodžio nustatymo iš naujo atgalinį įrašymą, pirmiausia įgalinkite „Azure AD Connect“ atgalinio rašymo parinktį. Iš savo „Azure AD Connect“ serverio, atlikite toliau pateiktus veiksmus:

1. Prisijunkite prie savo „Azure AD Connect“ serverio ir įjunkite **„Azure AD Connect“** konfigūravimo vediklį.
2. **Darbo pradžios** puslapyje, spustelėkite **Konfigūruoti**.
3. Puslapyje **Papildomos užduotys** pasirinkite **Tinkinti sinchronizavimo parinktis**, tuomet spustelėkite **Toliau**.
4. Puslapyje **Prisijungti prie „Azure AD“** įveskite visuotinio administratoriaus kredencialus savo „Azure“ klientui, o tuomet spustelėkite **Toliau**.
5. **Katalogų prijungimo** ir **Domeno/OU** filtravimo puslapiuose spustelėkite **Toliau**.
6. Puslapyje **Pasirenkamos funkcijos** pažymėkite langelį, esantį šalia **Slaptažodžio atgalinis įrašymas** ir spustelėkite **Toliau**.
7. Puslapyje **Paruošta konfigūruoti** spustelėkite **Konfigūruoti** ir palaukite, kol procesas bus baigtas.
8. Kai pamatysite, kad konfigūracija baigta, spustelėkite **Išeiti**.

Įgalinę „Azure AD Connect“ slaptažodžių atgalinį įrašymą, konfigūruokite „Azure AD“ SSPR atgaliniam rašymui.  Norėdami įgalinti atgalinį įrašymą SSPR, atlikite toliau pateiktus veiksmus:

1. Prisijunkite prie „Azure“ portalo naudodami visuotinio administratoriaus paskyrą.
2. Raskite ir pasirinkite **„Azure Active Directory“**, spustelėkite **Slaptažodžio nustatymas iš naujo**, tada – **Vietinis integravimas**.
3. Nustatykite parinktį **Įrašyti slaptažodžius į vietinį katalogą?** į **Taip**.
4. Nustatykite parinktį **Leisti vartotojams atrakinti paskyras nenustačius jų slaptažodžio iš naujo?** į **Taip**.
5. Kai baigsite, spustelėkite **Įrašyti**.

Daugiau informacijos žr. [„Azure Active Directory“ savitarnos slaptažodžio nustatymo iš naujo atgalinis įrašymas į vietinę aplinką](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Kai administratorius iš naujo nustato vartotojo slaptažodį „Azure“ portale, jei tas vartotojas yra išorinis arba slaptažodžio maiša sinchronizuota, slaptažodis įrašomas į vietinę versiją. Ši funkcija šiuo metu nepalaikoma „Office“ administravimo portale.