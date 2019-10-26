---
title: Problemos su MFP
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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545181"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="fe88a-102">Problemos su MFP</span><span class="sxs-lookup"><span data-stu-id="fe88a-102">Issues with MFA</span></span>
<span data-ttu-id="fe88a-103">Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudojant kelių dalių autentifikavimas (DTS)</span><span class="sxs-lookup"><span data-stu-id="fe88a-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="fe88a-104">Susijusio vartotojo gali būti užblokuotas Azure Active Directory portale.</span><span class="sxs-lookup"><span data-stu-id="fe88a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="fe88a-105">Tokiu atveju autentifikavimas bando, kad konkretus vartotojas bus automatiškai atmestas.</span><span class="sxs-lookup"><span data-stu-id="fe88a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="fe88a-106">Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="fe88a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="fe88a-107">Jei atblokavimo vartotojas nepadėjo arba vartotojas nėra užblokuotas galite pabandyti iš naujo MFP vartotojo ir jie bus eiti per Registruotis procesas dar kartą.</span><span class="sxs-lookup"><span data-stu-id="fe88a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="fe88a-108">Atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="fe88a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="fe88a-109">Jei tai pirmas kartas, kai įjungėte DTS ir jūsų vartotojai negali prisijungti prie ne naršyklės klientams, pvz., "Outlook", "Skype" ir tt, galbūt Alma (Active Directory autentifikavimo biblioteka) neįgalintas jūsų O365 prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="fe88a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="fe88a-110">Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir paleisti šį cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="fe88a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>