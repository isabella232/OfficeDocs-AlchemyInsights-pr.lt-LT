---
title: Vienas iš jūsų vietinių susiejimo tarnybos sertifikatų baigia galioti
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673505"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="348c4-102">Vienas iš jūsų vietinių susiejimo tarnybos sertifikatų baigia galioti</span><span class="sxs-lookup"><span data-stu-id="348c4-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="348c4-103">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="348c4-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="348c4-104">"Microsoft Azure Active Directory" modulio, skirto "Windows PowerShell", diegimas kompiuteryje (jei modulis dar neįdiegtas).</span><span class="sxs-lookup"><span data-stu-id="348c4-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="348c4-105">Norėdami tai padaryti, eikite į " [Azure Active Directory](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) " "PowerShell" diagrama</span><span class="sxs-lookup"><span data-stu-id="348c4-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="348c4-106">Vadovaukitės veiksmais, pateikiamais "1 scenarijus:" AD FS "atpažinimo ženklo patvirtinimo sertifikato galiojimas baigėsi" sekcija "įvyko [klaida jungiantis prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Microsoft 365", "Azure" arba "Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)".</span><span class="sxs-lookup"><span data-stu-id="348c4-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="348c4-107">Atlikite veiksmus, aprašytus [kaip atnaujinti arba pataisyti išorinio domeno parametrus programoje "Microsoft 365", "Azure" arba "Intune"](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="348c4-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="348c4-108">Daugiau informacijos apie tai, kaip atnaujinti susiejimo sertifikatus, ieškokite " [O365" ir "AZURE AD" sertifikato atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="348c4-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

