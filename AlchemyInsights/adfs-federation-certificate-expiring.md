---
title: ADFS susiejimo sertifikatas baigiasi
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952977"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS susiejimo sertifikatas baigiasi

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:
  
1. Įdiekite "Microsoft Azure Active Directory" modulio Windows PowerShell kompiuteryje (jei modulis dar neįdiegtas). Norėdami tai padaryti, eikite į ["Azure AD" valdymas naudojant Windows PowerShell](https://aka.ms/aadposh).

2. Atlikite veiksmus, nurodytus klaidos "1 scenarijus: BAIGĖSI AD FS atpažinimo ženklo pasirašymo sertifikato galiojimas" dalyje "Kilo problema bandant pasiekti svetainę" iš AD FS, kai išorinis vartotojas prisijungia [prie "Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Atlikite veiksmus, nurodytus išorinio domeno parametrų naujinimas arba atkūrimas ["Microsoft", "Azure" arba "Intune".](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Norėdami sužinoti daugiau apie susiejimo sertifikatų atnaujinimą, žr. Susiejimo sertifikatų [atnaujinimas Microsoft 365 ir "Azure Active Directory".](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
