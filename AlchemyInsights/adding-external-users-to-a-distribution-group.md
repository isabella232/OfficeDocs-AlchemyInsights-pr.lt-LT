---
title: Išorinių vartotojų įtraukimas į paskirstymo grupę
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910940"
---
# <a name="add-external-users-to-a-distribution-group"></a>Išorinių vartotojų įtraukimas į paskirstymo grupę

Išorinio kontakto įtraukimas į paskirstymo grupę (GD) yra dviejų etapų procesas:
  
1. Sukurkite išorinio vartotojo pašto kontaktą:
    
    1. Administravimo centre eikite į puslapį **Vartotojų** > [kontaktai.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Pasirinkite **Įtraukti adresatą**.
    
    3. Įveskite adresato informaciją ir pasirinkite **Įtraukti**.
    
2. Įtraukite pašto kontaktą į savo GENERALINĮ DIREKTORATĄ:
    
    1. Administravimo centre eikite į puslapį **Grupių** > [grupės.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Raskite GD, į kurį norite įtraukti išorinį vartotoją, ir pasirinkite jį, kad atidarytumėte redagavimo dialogo langą.
    
    3. Skirtuke **Nariai** pasirinkite **Peržiūrėti visus ir tvarkyti narius**. 
    
    4. Pasirinkite **Įtraukti narius**.
    
    5. Pasirinkite pašto kontaktą, kurį sukūrėte atlikdami ankstesnį veiksmą, tada pasirinkite **Įrašyti**.
    
Jei atlikus šiuos veiksmus išoriniai vartotojai negali siųsti el. laiškų GENERALINIAM DIREKTORATUI arba iš jo negauti el. laiškų, gali būti, kad GD pažymėtas taip, kad leistų siųsti tik vidinių naudotojų el. laiškus. Galite patikrinti šią konfigūraciją ir pataisyti ją pagal nuorodas [čia](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Pastaba:** Šios instrukcijos netaikomos, jei jūsų grupės tipas yra "Microsoft 365 grupė", o ne "Paskirstymo grupė". Tokiu atveju išorinį vartotoją galite įtraukti tiesiai į grupę iš "Outlook". Išsamią informaciją apie "Microsoft 365 Groups" svečius ir išorinių svečių įtraukimo instrukcijas rasite [šiame straipsnyje](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  