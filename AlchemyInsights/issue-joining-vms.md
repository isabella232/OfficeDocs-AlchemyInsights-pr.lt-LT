---
title: Problemos prisijungiant prie VM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885668"
---
# <a name="issue-joining-vms"></a>Problemos prisijungiant prie VM

Norėdami išspręsti problemas, kylančias bandant prisijungti prie VM, atlikite šiuos veiksmus:

1. Pabandykite prisijungti naudodami **UPN** formatą (pvz., "joeuser@contoso.com"), o ne " **sAMAccountName** " formatą ("Contoso\joe vartotojas").
2. Įsitikinkite, kad įgalinote slaptažodžių sinchronizavimą pagal veiksmus, nurodytus *darbo pradžios* vadove.
3. Įsitikinkite, kad paveikto vartotojo abonementas nėra išorinis "Azure AD" nuomotojo abonementas. Išoriniai vartotojai negali prisijungti prie valdomo domeno, nes "Azure AD domain Services" neturi kredencialų tokiems vartotojų abonementams.
4. Jei paveikto vartotojo abonementas yra tik debesies vartotojo abonementas, įsitikinkite, kad vartotojai pakeitė savo slaptažodį įgalinę "Azure AD domain Services". Atlikus šį veiksmą, reikia sugeneruoti "Azure AD" domenų tarnyboms būtiną kredencialų maišos funkciją.
5. Jei pažeistos vartotojų paskyros sinchronizuojamos iš vietinio katalogo, patikrinkite, ar rekomenduojama "Azure AD Connect" versija sukonfigūruota atlikti visas sinchronizacijos funkcijas.
6. Jei po 4 veiksmo patvirtinimo problemos kartosis, vykdykite šias komandas iš savo sinchronizavimo kompiuterio:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.