---
title: Slaptažodžio sinchronizavimo trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924704"
---
# <a name="troubleshoot-password-synchronization"></a>Slaptažodžio sinchronizavimo trikčių šalinimas

Norėdami išspręsti problemas, kai slaptažodžių yra sinchronizuota su Azure AD Connect versija 1.1.614.0 arba naujesnė versija:
  
1. Atidarykite naują "Windows PowerShell" seansą "Azure AD Connect" serveryje naudojant parinktį **paleisti kaip administratoriui** . 
    
2. Vykdykite **Set-ExecutionPolicy RemoteSigned** arba **Set-ExecutionPolicy neribojamas**. 
    
3. Paleisti Azure AD Connect vedlį.
    
4. Eikite į į ** papildomas užduotis ** puslapyje, pasirinkite ** trikčių šalinimas **, ir spustelėkite **Pirmyn**. 
    
5. Puslapio trikčių šalinimas, spustelėkite meniu **Pradėti pradėti trikčių šalinimas** "PowerShell". 
    
6. Pagrindiniame meniu pasirinkite **Šalinti triktis slaptažodžių sinchronizavimas**. 
    
7. Submeniu, pasirinkite **slaptažodžio sinchronizavimo neveikia ne visiems**. 
    
 **Suprasti trikčių šalinimo užduoties rezultatai**
  
Trikčių šalinimo užduotį atlieka šiuos patikrinimus:
  
- Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungtas savo Azure AD nuomotojo.
    
- Patvirtina, kad Azure AD Connect serveris nėra – sustojimo režimu.
    
- Už kiekvieną esamą vietinės Active Directory jungties (kuris atitinka esamo Active Directory miško):
    
- 
  - Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungta.
    
  - Ieško slaptažodžio sinchronizavimo širdies plakimas įvykius Windows programos įvykių žurnale.
    
  - Kiekvieno Active Directory domeno pagal vietinės Active Directory jungtis:
    
  - Patvirtina, kad domenas yra pasiekiamas iš Azure AD Connect serverio.
    
  - Patvirtina, kad Active Directory domenų tarnybos (AD DS) sąskaitų, naudojamų vietinių Active Directory jungtis turi teisingą vartotojo vardą, slaptažodį ir slaptažodį Sinchronizacijai reikalingus leidimus.
    
Daugiau pagalbos dėl slaptažodžio Sinchronizavimo trikčių šalinimas, žr [Šalinti triktis slaptažodžių sinchronizavimas su sinchronizavimo Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

