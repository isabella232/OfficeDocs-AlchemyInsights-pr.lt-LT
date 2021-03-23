---
title: Tarnybos jungties taško (SCP) konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036146"
---
# <a name="configure-service-connection-point-scp"></a>Tarnybos jungties taško (SCP) konfigūravimas

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Priežastis**: nepavyko perskaityti SCP objekto ir gauti "Azure AD" nuomotojo informaciją
- **Skiriamoji geba**: ieškokite skyriaus [tarnybos kreipties taško konfigūravimas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Veiksmų planas**

- Patikrinkite, ar įrenginys gavo GPO, skirtą valdomam patvirtinimui.
- Įsitikinkite, kad GPO sukūrė registro raktus.
- Įsitikinkite, kad turite 2 raktus, sukurtus naudojant katalogo ID ir "onmicrosoft domain".

**Konfigūruoti kliento pusės registro parametrą, skirtą "SCP"**

Naudokite toliau pateiktą pavyzdį, kad sukurtumėte grupės strategijos objektą (GPO), kad galėtumėte įdiegti registro parametrą, kuris konfigūruoja SCP įrašą jūsų įrenginių registre.

1. Atidarykite grupės strategijos valdymo konsolę ir sukurkite naują GPO savo domene.
     - Pateikite naujai sukurtą GPO vardą (pvz., ClientSideSCP)

2. Redaguoti GPO ir rasti šį kelią: **kompiuterio konfigūracija > nuostatos > "Windows" parametrų > registrą**.

3. Dešiniuoju pelės mygtuku spustelėkite **registrą** ir pasirinkite **naujas > registro elementą**.

4. Skirtuke **Bendrasis** Konfigūruokite šiuos dalykus:
  
- **Veiksmas**: naujinimas
    
- **Avilys**: HKEY_LOCAL_MACHINE
    
- **Rakto Path**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Reikšmės pavadinimas**: tenantid
    
- **Reikšmės tipas**: REG_SZ
    
- **Reikšmės duomenys**: "Azure AD" egzemplioriaus GUID arba katalogo ID (šią reikšmę galima rasti "Azure" **portale > "Azure Active Directory" > ypatybių > katalogo ID**)
 
- Spustelėkite **Gerai**.
 
5. Dešiniuoju pelės mygtuku spustelėkite **registrą** ir pasirinkite **naujas > registro elementą**.

6. Skirtuke **Bendrasis** Konfigūruokite šiuos dalykus:
  
- **Veiksmas**: naujinimas
    
- **Avilys**: HKEY_LOCAL_MACHINE
    
- **Rakto Path**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Reikšmės pavadinimas**: tenantname
    
- **Reikšmės tipas**: REG_SZ
    
- **Reikšmės duomenys**: jūsų patvirtintas domeno vardas, jei naudojate bendrą aplinką, pvz., AD FS. Jūsų patvirtintas domeno vardas arba onmicrosoft.com domeno vardas (pvz., contoso. onmicrosoft). com, jei naudojate valdomą aplinką

- Spustelėkite **Gerai**.

7. Uždarykite naujai sukurto GPO rengyklę.

8. Susiekite naujai sukurtą GPO su pageidaujamu OU, kuriame yra domeno sujungti kompiuteriai, priklausantys jūsų kontroliuojamam "rida" populiacijai.

Daugiau informacijos ieškokite " [hibridinio" AZURE ad Join-AZURE AD "kontroliuojamo tikrinimo tikrinimas | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) ir  [trikčių diagnostikos hibridiniai "Azure Active Directory" sujungti įrenginiai | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









