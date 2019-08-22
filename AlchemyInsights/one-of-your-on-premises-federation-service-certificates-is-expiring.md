---
title: Vienas iš jūsų vietinio federacijos paslaugų sertifikatai nustos galioti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543573"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Vienas iš jūsų vietinio federacijos paslaugų sertifikatai nustos galioti

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
- Įdiegti į "Microsoft" Azure Active Directory modulis už "Windows PowerShell" kompiuteryje (jei modulis nėra įdiegta). Norėdami tai padaryti, eikite į [Azure Active Directory PowerShell grafikas](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Atlikite veiksmus į "1 scenarijus: AD FS atpažinimo ženklas pasirašymo sertifikato galiojimo pabaigos" skyriuje ["Ten buvo problema prieinant prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Office 365", Azure, ar Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Vykdykite t[kaip atnaujinti arba pataisyti išorinio domeno "Office 365", Azure, ar Intune parametrus](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Daugiau informacijos apie atnaujinimo federacijos sertifikatai, rasite [sertifikato atnaujinimo O365 ir Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

