---
title: Išorinių vartotojų įtraukimas į platinimo grupę
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663521"
---
# <a name="add-external-users-to-a-distribution-group"></a>Išorinių vartotojų įtraukimas į platinimo grupę

Išorinio kontakto įtraukimas į platinimo grupę (DG) yra dviejų etapų procesas:
  
1. Išorinio vartotojo pašto kontakto kūrimas:
    
    1. Administravimo centre eikite į puslapį **vartotojų**  >  [Kontaktai](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Pasirinkite **įtraukti kontaktą**.
    
    3. Įveskite kontakto informaciją ir pasirinkite **įtraukti**.
    
2. Įtraukite pašto kontaktą į savo GD:
    
    1. Administravimo centre eikite į puslapį **grupių**  >  [grupės](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Raskite generalinį direktoratą, į kurį norite įtraukti išorinį vartotoją, ir pasirinkite jį, kad atidarytumėte dialogo langą redagavimas.
    
    3. Skirtuke **nariai** pasirinkite **Peržiūrėti visus ir valdykite narius**. 
    
    4. Pasirinkite **įtraukti narius**.
    
    5. Pasirinkite pašto kontaktą, kurį sukūrėte atlikdami ankstesnį veiksmą, tada pasirinkite **įrašyti**.
    
Jei atlikus šiuos veiksmus, Išoriniai vartotojai negali siųsti el. laiškų generaliniam direktoratui arba negauna iš jo gautų laiškų, gali būti, kad GD yra pažymėtas tik leisti laiškus iš vidinių vartotojų. Galite patikrinti šį konfigūravimą ir ją pataisyti vykdydami nurodymus [čia](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Pastaba:** Šios instrukcijos netaikomos, jei jūsų grupės tipas yra "Microsoft 365 Group", o ne "Distribution Group". Jei tai yra atvejis, galite tiesiogiai įtraukti išorinį vartotoją į grupę iš "Outlook". Išsamios informacijos apie "Microsoft" 365 grupių svečių ir išorinių Svečių įtraukimo instrukcijas rasite [šiame straipsnyje](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  