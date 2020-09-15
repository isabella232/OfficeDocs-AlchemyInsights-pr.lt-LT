---
title: ADFS susiejimo sertifikato galiojimas baigiasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686722"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS susiejimo sertifikato galiojimas baigiasi

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
1. "Microsoft Azure Active Directory" modulio, skirto "Windows PowerShell", diegimas kompiuteryje (jei modulis dar neįdiegtas). Norėdami tai padaryti, eikite į ["AZURE AD" valdymas naudojant "Windows PowerShell"](https://aka.ms/aadposh).

2. Vadovaukitės veiksmais, pateikiamais "1 scenarijus:" AD FS "atpažinimo ženklo patvirtinimo sertifikato galiojimas baigėsi" sekcija "įvyko [klaida jungiantis prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Microsoft 365", "Azure" arba "Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)".

3. Atlikite veiksmus, aprašytus dalyje ["Microsoft", "Azure" arba "Intune" išorinio domeno parametrų naujinimas arba taisymas](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Jei norite daugiau sužinoti apie "Federation" sertifikatų atnaujinimą, skaitykite ["Microsoft 365" ir "Azure Active Directory" susiejimo sertifikatų atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
