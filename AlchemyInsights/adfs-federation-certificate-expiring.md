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
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662371"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a7da0-102">ADF federacijos pažymėjimas baigiasi</span><span class="sxs-lookup"><span data-stu-id="a7da0-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a7da0-103">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a7da0-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a7da0-p101">Įdiegti į "Microsoft" Azure Active Directory modulis už "Windows PowerShell" kompiuteryje (jei modulis nėra įdiegta). Norėdami tai padaryti, eikite į [valdyti Azure AD naudojant "Windows PowerShell"](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="a7da0-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="a7da0-106">Atlikite veiksmus į "1 scenarijus: AD FS atpažinimo ženklas pasirašymo sertifikato galiojimo pabaigos" skyriuje ["Ten buvo problema prieinant prie svetainės" klaida iš AD FS, kai išorinis vartotojas prisijungia prie "Office 365", Azure, ar Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a7da0-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="a7da0-107">Atlikite veiksmus, [kaip atnaujinti arba pataisyti išorinio domeno "Office 365", Azure, ar Intune parametrus](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="a7da0-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="a7da0-108">Norėdami sužinoti daugiau apie atnaujinimo federacijos sertifikatus, pamatyti [atnaujinti "Office 365" ir Azure Active Directory Federacijos liudijimai](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a7da0-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

