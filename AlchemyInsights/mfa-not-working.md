---
title: Problemas, susijusias su URM
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250173"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="51a5f-102">Problemas, susijusias su URM</span><span class="sxs-lookup"><span data-stu-id="51a5f-102">Issues with MFA</span></span>
<span data-ttu-id="51a5f-103">Yra keletas dalykų, kuriuos reikia patikrinti, jei vartotojai negali prisijungti naudodami kelių dalių autentifikavimas (DTS)</span><span class="sxs-lookup"><span data-stu-id="51a5f-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="51a5f-104">Įtakos vartotojas gali būti blokuojami Azure Active Directory portale.</span><span class="sxs-lookup"><span data-stu-id="51a5f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="51a5f-105">Jei tai byla, autentifikavimo bandymų, kad konkrečiam vartotojui bus automatiškai atmesti.</span><span class="sxs-lookup"><span data-stu-id="51a5f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="51a5f-106">Atlikite veiksmus šiame straipsnyje, atblokuoti juos.</span><span class="sxs-lookup"><span data-stu-id="51a5f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="51a5f-107">Jei vartotojo atblokavimas nepadėjo arba vartotojas nėra užblokuota galite bandyti iš naujo URM vartotojas ir jie bus eiti per Registruotis procesą dar kartą.</span><span class="sxs-lookup"><span data-stu-id="51a5f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="51a5f-108">Atlikite veiksmus šiame straipsnyje.</span><span class="sxs-lookup"><span data-stu-id="51a5f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="51a5f-109">Jei tai pirmas kartas, tu įgalintas MFP ir vartotojams negalite prisijungti prie naršyklės Klientai pvz., "Outlook", "Skype" ir t.t., gal Alma (Active Directory autentifikavimo bibliotekos) nėra įjungtas prenumeratą O365.</span><span class="sxs-lookup"><span data-stu-id="51a5f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="51a5f-110">Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir vykdyti šį cmdlet:  *Set-OrganizationalSetting-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="51a5f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>