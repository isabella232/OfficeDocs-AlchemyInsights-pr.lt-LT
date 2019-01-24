---
title: ADF federacijos pažymėjimas baigiasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480738"
---
# <a name="adfs-federation-certificate-expiring"></a>ADF federacijos pažymėjimas baigiasi

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
1. Įdiegti į "Microsoft" Azure Active Directory modulis už "Windows PowerShell" kompiuteryje (jei modulis nėra įdiegta). Norėdami tai padaryti, eikite į [valdyti Azure AD naudojant "Windows PowerShell"](https://aka.ms/aadposh).
    
2. Atlikite veiksmus į "1 scenarijus: AD FS atpažinimo ženklas pasirašymo sertifikato galiojimo pabaigos" skyriuje ["Ten buvo problema prieinant prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Office 365", Azure, ar Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Atlikite veiksmus, [kaip atnaujinti arba pataisyti išorinio domeno "Office 365", Azure, ar Intune parametrus](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Norėdami sužinoti daugiau apie atnaujinimo federacijos sertifikatus, pamatyti [atnaujinti "Office 365" ir Azure Active Directory Federacijos liudijimai](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

