---
title: Slaptažodžio sinchronizavimo trikčių šalinimas
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
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767184"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="3f88e-102">Slaptažodžio sinchronizavimo trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="3f88e-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="3f88e-103">Norėdami išspręsti problemas, kai slaptažodžių yra sinchronizuota su Azure AD Connect versija 1.1.614.0 arba naujesnė versija:</span><span class="sxs-lookup"><span data-stu-id="3f88e-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="3f88e-104">Atidarykite naują "Windows PowerShell" seansą "Azure AD Connect" serveryje naudojant parinktį **paleisti kaip administratoriui** .</span><span class="sxs-lookup"><span data-stu-id="3f88e-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="3f88e-105">Vykdykite **Set-ExecutionPolicy RemoteSigned** arba **Set-ExecutionPolicy neribojamas**.</span><span class="sxs-lookup"><span data-stu-id="3f88e-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="3f88e-106">Paleisti Azure AD Connect vedlį.</span><span class="sxs-lookup"><span data-stu-id="3f88e-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="3f88e-107">Eikite į į \*\* papildomas užduotis \*\* puslapyje, pasirinkite \*\* trikčių šalinimas \*\*, ir spustelėkite **Pirmyn**.</span><span class="sxs-lookup"><span data-stu-id="3f88e-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="3f88e-108">Puslapio trikčių šalinimas, spustelėkite meniu **Pradėti pradėti trikčių šalinimas** "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="3f88e-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="3f88e-109">Pagrindiniame meniu pasirinkite **Šalinti triktis slaptažodžių sinchronizavimas**.</span><span class="sxs-lookup"><span data-stu-id="3f88e-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="3f88e-110">Submeniu, pasirinkite **slaptažodžio sinchronizavimo neveikia ne visiems**.</span><span class="sxs-lookup"><span data-stu-id="3f88e-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="3f88e-111">**Suprasti trikčių šalinimo užduoties rezultatai**</span><span class="sxs-lookup"><span data-stu-id="3f88e-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="3f88e-112">Trikčių šalinimo užduotį atlieka šiuos patikrinimus:</span><span class="sxs-lookup"><span data-stu-id="3f88e-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="3f88e-113">Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungtas savo Azure AD nuomotojo.</span><span class="sxs-lookup"><span data-stu-id="3f88e-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="3f88e-114">Patvirtina, kad Azure AD Connect serveris nėra – sustojimo režimu.</span><span class="sxs-lookup"><span data-stu-id="3f88e-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="3f88e-115">Už kiekvieną esamą vietinės Active Directory jungties (kuris atitinka esamo Active Directory miško):</span><span class="sxs-lookup"><span data-stu-id="3f88e-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="3f88e-116">Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungta.</span><span class="sxs-lookup"><span data-stu-id="3f88e-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="3f88e-117">Ieško slaptažodžio sinchronizavimo širdies plakimas įvykius Windows programos įvykių žurnale.</span><span class="sxs-lookup"><span data-stu-id="3f88e-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="3f88e-118">Kiekvieno Active Directory domeno pagal vietinės Active Directory jungtis:</span><span class="sxs-lookup"><span data-stu-id="3f88e-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="3f88e-119">Patvirtina, kad domenas yra pasiekiamas iš Azure AD Connect serverio.</span><span class="sxs-lookup"><span data-stu-id="3f88e-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="3f88e-120">Patvirtina, kad Active Directory domenų tarnybos (AD DS) sąskaitų, naudojamų vietinių Active Directory jungtis turi teisingą vartotojo vardą, slaptažodį ir slaptažodį Sinchronizacijai reikalingus leidimus.</span><span class="sxs-lookup"><span data-stu-id="3f88e-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="3f88e-121">Daugiau pagalbos dėl slaptažodžio Sinchronizavimo trikčių šalinimas, žr [Šalinti triktis slaptažodžių sinchronizavimas su sinchronizavimo Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3f88e-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

