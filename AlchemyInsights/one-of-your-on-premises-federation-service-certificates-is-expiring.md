---
title: Vienas iš jūsų vietinės susiejimo tarnybos sertifikatų baigiasi
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810060"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="e5c6b-102">Vienas iš jūsų vietinės susiejimo tarnybos sertifikatų baigiasi</span><span class="sxs-lookup"><span data-stu-id="e5c6b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="e5c6b-103">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="e5c6b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="e5c6b-104">Kompiuteryje įdiekite "Microsoft Azure Active Directory" modulį, skirtą "Windows PowerShell" (jei modulis dar neįdiegtas).</span><span class="sxs-lookup"><span data-stu-id="e5c6b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="e5c6b-105">Norėdami tai padaryti, eikite į ["Azure Active Directory PowerShell for Graph" ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="e5c6b-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="e5c6b-106">Atlikite veiksmus, nurodytus skyriuje "1 scenarijus: baigėsi "AD FS atpažinimo ženklo pasirašymo sertifikato galiojimas", kai išorinis vartotojas prisijungia prie ["Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="e5c6b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="e5c6b-107">Atlikite veiksmus, nurodytus Kaip atnaujinti arba atkurti išorinio domeno parametrus ["Microsoft 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="e5c6b-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="e5c6b-108">Daugiau informacijos apie susiejimo sertifikatų atnaujinimą žr. ["O365" ir "Azure AD" sertifikatų atnaujinimas.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="e5c6b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

