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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="70a9c-102">ADFS susiejimo sertifikato galiojimas baigiasi</span><span class="sxs-lookup"><span data-stu-id="70a9c-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="70a9c-103">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="70a9c-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="70a9c-104">"Microsoft Azure Active Directory" modulio, skirto "Windows PowerShell", diegimas kompiuteryje (jei modulis dar neįdiegtas).</span><span class="sxs-lookup"><span data-stu-id="70a9c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="70a9c-105">Norėdami tai padaryti, eikite į ["AZURE AD" valdymas naudojant "Windows PowerShell"](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="70a9c-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="70a9c-106">Vadovaukitės veiksmais, pateikiamais "1 scenarijus:" AD FS "atpažinimo ženklo patvirtinimo sertifikato galiojimas baigėsi" sekcija "įvyko [klaida jungiantis prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Microsoft 365", "Azure" arba "Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)".</span><span class="sxs-lookup"><span data-stu-id="70a9c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="70a9c-107">Atlikite veiksmus, aprašytus dalyje ["Microsoft", "Azure" arba "Intune" išorinio domeno parametrų naujinimas arba taisymas](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="70a9c-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="70a9c-108">Jei norite daugiau sužinoti apie "Federation" sertifikatų atnaujinimą, skaitykite ["Microsoft 365" ir "Azure Active Directory" susiejimo sertifikatų atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="70a9c-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
