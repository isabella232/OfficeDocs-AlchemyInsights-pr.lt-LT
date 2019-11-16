---
title: ADFS susiejimo sertifikato galiojimo pabaiga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737197"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS susiejimo sertifikato galiojimo pabaiga

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
1. Kompiuteryje įdiekite "Microsoft Azure Active Directory" modulį, skirtą "Windows PowerShell" (jei modulis dar neįdiegtas). Norėdami tai padaryti, eikite į [valdyti AZURE ad naudojant "Windows PowerShell"](https://aka.ms/aadposh).

2. Atlikite veiksmus, nurodytus "scenarijų 1: AD FS atpažinimo ženklas pasirašymo sertifikato galiojimas" skyriuje ["kilo problema bandant pasiekti svetainę" klaida iš AD FS, kai išorinis vartotojas prisijungia prie Office 365, Azure arba Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Vykdykite [naujinimą arba pataisykite išorinio domeno parametrus Office 365, Azure arba Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Jei norite sužinoti daugiau apie susiejimo sertifikatų atnaujinimą, peržiūrėkite " [Office 365" ir "Azure Active Directory" susiejimo sertifikatų atnaujinimą](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
