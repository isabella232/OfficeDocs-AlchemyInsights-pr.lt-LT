---
title: Slaptažodžių sinchronizavimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732518"
---
# <a name="troubleshoot-password-synchronization"></a>Slaptažodžių sinchronizavimo trikčių diagnostika

Norėdami išspręsti problemas, kai nėra slaptažodžių sinchronizuojami su Azure AD Connect versija 1.1.614.0 arba naujesnė versija:
  
1. Atidarykite naują "Windows PowerShell" seansą savo Azure AD Connect serveryje su **parinktimi paleisti administratoriaus teisėmis** .

2. Vykdyti **Set-ExecutionPolicy RemoteSigned** arba **Set-ExecutionPolicy neribotas**.

3. Paleiskite Azure AD Connect vedlį.

4. Eikite į **puslapį Papildomos užduotys,** pasirinkite **Šalinti triktis**ir spustelėkite **Pirmyn**.

5. Puslapyje Trikčių diagnostika spustelėkite **Paleisti, kad paleistumėte "PowerShell" trikčių diagnostikos** meniu.

6. Pagrindiniame meniu pasirinkite **Šalinti slaptažodžių sinchronizavimo triktis**.

7. Submeniu pasirinkite **Slaptažodžių sinchronizavimas neveikia .**

**Trikčių šalinimo užduoties rezultatų supratimas**
  
Trikčių šalinimo užduotis atlieka šiuos patikrinimus:
  
- Patikrina, ar slaptažodžio sinchronizavimo funkcija yra įjungta jūsų Azure AD nuomotojo.

- Patikrina, ar Azure AD Connect serveris nėra sustojimo režimu.

- Kiekvienam esamam vietiniam active Directory jungtis (kuri atitinka esamą Active Directory miško):

- 
  - Patikrina, ar įjungta slaptažodžio sinchronizavimo funkcija.

  - Ieško slaptažodžio sinchronizavimo širdies plakimas įvykių Windows programos įvykių žurnaluose.

  - Kiekvienam Active Directory domeno vietiniame Active Directory jungtis:

  - Patikrina, ar domenas pasiekiamas iš Azure AD Connect serverio.

  - Patikrina, ar "Active Directory" domenų tarnybos (AD DS) abonementai, kuriuos naudoja vietinė "Active Directory" jungtis, turi teisingą vartotojo vardą, slaptažodį ir teises, reikalingas slaptažodžio sinchronizavimui.

Daugiau pagalbos slaptažodžio sinchronizavimo trikčių diagnostika ieškokite [Slaptažodžių sinchronizavimo trikčių diagnostika naudojant "Azure AD Connect" sinchronizavimą](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  