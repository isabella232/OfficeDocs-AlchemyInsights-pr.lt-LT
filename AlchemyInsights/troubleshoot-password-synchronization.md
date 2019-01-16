---
title: Slaptažodžio sinchronizavimo trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301980"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e790f-102">Slaptažodžio sinchronizavimo trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="e790f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e790f-103">Norėdami išspręsti problemas, kai slaptažodžių yra sinchronizuota su Azure AD Connect versija 1.1.614.0 arba naujesnė versija:</span><span class="sxs-lookup"><span data-stu-id="e790f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e790f-104">Atidarykite naują "Windows PowerShell" seansą "Azure AD Connect" serveryje naudojant parinktį **paleisti kaip administratoriui** .</span><span class="sxs-lookup"><span data-stu-id="e790f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="e790f-105">Vykdykite **Set-ExecutionPolicy RemoteSigned** arba **Set-ExecutionPolicy neribojamas**.</span><span class="sxs-lookup"><span data-stu-id="e790f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="e790f-106">Paleisti Azure AD Connect vedlį.</span><span class="sxs-lookup"><span data-stu-id="e790f-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="e790f-107">Eikite į į \*\* papildomas užduotis \*\* puslapyje, pasirinkite \*\* trikčių šalinimas \*\*, ir spustelėkite **Pirmyn**.</span><span class="sxs-lookup"><span data-stu-id="e790f-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="e790f-108">Puslapio trikčių šalinimas, spustelėkite meniu **Pradėti pradėti trikčių šalinimas** "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="e790f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="e790f-109">Pagrindiniame meniu pasirinkite **Šalinti triktis slaptažodžių sinchronizavimas**.</span><span class="sxs-lookup"><span data-stu-id="e790f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="e790f-110">Submeniu, pasirinkite **slaptažodžio sinchronizavimo neveikia ne visiems**.</span><span class="sxs-lookup"><span data-stu-id="e790f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="e790f-111">**Suprasti trikčių šalinimo užduoties rezultatai**</span><span class="sxs-lookup"><span data-stu-id="e790f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e790f-112">Trikčių šalinimo užduotį atlieka šiuos patikrinimus:</span><span class="sxs-lookup"><span data-stu-id="e790f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e790f-113">Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungtas savo Azure AD nuomotojo.</span><span class="sxs-lookup"><span data-stu-id="e790f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="e790f-114">Patvirtina, kad Azure AD Connect serveris nėra – sustojimo režimu.</span><span class="sxs-lookup"><span data-stu-id="e790f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="e790f-115">Už kiekvieną esamą vietinės Active Directory jungties (kuris atitinka esamo Active Directory miško):</span><span class="sxs-lookup"><span data-stu-id="e790f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="e790f-116">Patvirtina, kad slaptažodžio sinchronizavimo funkcija yra įjungta.</span><span class="sxs-lookup"><span data-stu-id="e790f-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="e790f-117">Ieško slaptažodžio sinchronizavimo širdies plakimas įvykius Windows programos įvykių žurnale.</span><span class="sxs-lookup"><span data-stu-id="e790f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="e790f-118">Kiekvieno Active Directory domeno pagal vietinės Active Directory jungtis:</span><span class="sxs-lookup"><span data-stu-id="e790f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="e790f-119">Patvirtina, kad domenas yra pasiekiamas iš Azure AD Connect serverio.</span><span class="sxs-lookup"><span data-stu-id="e790f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="e790f-120">Patvirtina, kad Active Directory domenų tarnybos (AD DS) sąskaitų, naudojamų vietinių Active Directory jungtis turi teisingą vartotojo vardą, slaptažodį ir slaptažodį Sinchronizacijai reikalingus leidimus.</span><span class="sxs-lookup"><span data-stu-id="e790f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="e790f-121">Daugiau pagalbos dėl slaptažodžio Sinchronizavimo trikčių šalinimas, žr [Šalinti triktis slaptažodžių sinchronizavimas su sinchronizavimo Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e790f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

