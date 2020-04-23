---
title: Slaptažodžių sinchronizavimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732518"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="17949-102">Slaptažodžių sinchronizavimo trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="17949-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="17949-103">Norėdami išspręsti problemas, kai nėra slaptažodžių sinchronizuojami su Azure AD Connect versija 1.1.614.0 arba naujesnė versija:</span><span class="sxs-lookup"><span data-stu-id="17949-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="17949-104">Atidarykite naują "Windows PowerShell" seansą savo Azure AD Connect serveryje su **parinktimi paleisti administratoriaus teisėmis** .</span><span class="sxs-lookup"><span data-stu-id="17949-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="17949-105">Vykdyti **Set-ExecutionPolicy RemoteSigned** arba **Set-ExecutionPolicy neribotas**.</span><span class="sxs-lookup"><span data-stu-id="17949-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="17949-106">Paleiskite Azure AD Connect vedlį.</span><span class="sxs-lookup"><span data-stu-id="17949-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="17949-107">Eikite į **puslapį Papildomos užduotys,** pasirinkite **Šalinti triktis**ir spustelėkite **Pirmyn**.</span><span class="sxs-lookup"><span data-stu-id="17949-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="17949-108">Puslapyje Trikčių diagnostika spustelėkite **Paleisti, kad paleistumėte "PowerShell" trikčių diagnostikos** meniu.</span><span class="sxs-lookup"><span data-stu-id="17949-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="17949-109">Pagrindiniame meniu pasirinkite **Šalinti slaptažodžių sinchronizavimo triktis**.</span><span class="sxs-lookup"><span data-stu-id="17949-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="17949-110">Submeniu pasirinkite **Slaptažodžių sinchronizavimas neveikia .**</span><span class="sxs-lookup"><span data-stu-id="17949-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="17949-111">**Trikčių šalinimo užduoties rezultatų supratimas**</span><span class="sxs-lookup"><span data-stu-id="17949-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="17949-112">Trikčių šalinimo užduotis atlieka šiuos patikrinimus:</span><span class="sxs-lookup"><span data-stu-id="17949-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="17949-113">Patikrina, ar slaptažodžio sinchronizavimo funkcija yra įjungta jūsų Azure AD nuomotojo.</span><span class="sxs-lookup"><span data-stu-id="17949-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="17949-114">Patikrina, ar Azure AD Connect serveris nėra sustojimo režimu.</span><span class="sxs-lookup"><span data-stu-id="17949-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="17949-115">Kiekvienam esamam vietiniam active Directory jungtis (kuri atitinka esamą Active Directory miško):</span><span class="sxs-lookup"><span data-stu-id="17949-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="17949-116">Patikrina, ar įjungta slaptažodžio sinchronizavimo funkcija.</span><span class="sxs-lookup"><span data-stu-id="17949-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="17949-117">Ieško slaptažodžio sinchronizavimo širdies plakimas įvykių Windows programos įvykių žurnaluose.</span><span class="sxs-lookup"><span data-stu-id="17949-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="17949-118">Kiekvienam Active Directory domeno vietiniame Active Directory jungtis:</span><span class="sxs-lookup"><span data-stu-id="17949-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="17949-119">Patikrina, ar domenas pasiekiamas iš Azure AD Connect serverio.</span><span class="sxs-lookup"><span data-stu-id="17949-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="17949-120">Patikrina, ar "Active Directory" domenų tarnybos (AD DS) abonementai, kuriuos naudoja vietinė "Active Directory" jungtis, turi teisingą vartotojo vardą, slaptažodį ir teises, reikalingas slaptažodžio sinchronizavimui.</span><span class="sxs-lookup"><span data-stu-id="17949-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="17949-121">Daugiau pagalbos slaptažodžio sinchronizavimo trikčių diagnostika ieškokite [Slaptažodžių sinchronizavimo trikčių diagnostika naudojant "Azure AD Connect" sinchronizavimą](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="17949-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  