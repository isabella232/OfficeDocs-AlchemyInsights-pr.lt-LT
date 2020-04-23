---
title: Vienas iš jūsų vietinių susiejimo paslaugų sertifikatų baigiasi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785311"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="70d85-102">Vienas iš jūsų vietinių susiejimo paslaugų sertifikatų baigiasi</span><span class="sxs-lookup"><span data-stu-id="70d85-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="70d85-103">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="70d85-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="70d85-104">Įdiekite "Microsoft Azure Active Directory" modulį, skirtą "Windows PowerShell" kompiuteryje (jei modulis dar neįdiegtas).</span><span class="sxs-lookup"><span data-stu-id="70d85-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="70d85-105">Norėdami tai padaryti, eikite į [Azure Active Directory PowerShell graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="70d85-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="70d85-106">Atlikite veiksmus, nurodytus skyriuje "1 scenarijus: AD FS atpažinimo ženklų pasirašymo sertifikato galiojimo laikas baigėsi" [klaidos pranešimą "Iškilo problema bandant pasiekti svetainę" iš AD FS, kai išorinis vartotojas prisijungia prie "Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="70d85-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="70d85-107">Atlikite [veiksmus, kaip atnaujinti arba atkurti išorinio domeno parametrus "Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="70d85-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="70d85-108">Jei norite gauti daugiau informacijos apie atnaujinti susiejimo sertifikatai, peržiūrėkite [sertifikato atnaujinimo O365 ir Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="70d85-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

