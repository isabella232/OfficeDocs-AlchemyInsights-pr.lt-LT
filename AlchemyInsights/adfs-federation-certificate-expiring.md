---
title: ADFS susiejimo sertifikato galiojimo laikas
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
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710415"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS susiejimo sertifikato galiojimo laikas

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
1. Įdiekite "Microsoft Azure Active Directory" modulį, skirtą "Windows PowerShell" kompiuteryje (jei modulis dar neįdiegtas). Norėdami tai padaryti, eikite į [Tvarkyti Azure AD naudojant "Windows PowerShell".](https://aka.ms/aadposh)

2. Atlikite veiksmus, nurodytus skyriuje "1 scenarijus: AD FS atpažinimo ženklų pasirašymo sertifikato galiojimo laikas baigėsi" [klaidos pranešimą "Iškilo problema bandant pasiekti svetainę" iš AD FS, kai išorinis vartotojas prisijungia prie "Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Atlikite [veiksmus, nurodytus "Microsoft", "Azure" arba "Intune" išorinio domeno parametruose](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)naujinimas arba taisymas .

    Norėdami sužinoti daugiau apie susiejimo sertifikatų atnaujinimą, peržiūrėkite [Atnaujinti susiejimo sertifikatai Microsoft 365 ir Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
