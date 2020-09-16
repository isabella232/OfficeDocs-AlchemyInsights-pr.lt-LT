---
title: "\"MFA\" problemos"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755139"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="f37ed-102">"Azure MFA" problemos</span><span class="sxs-lookup"><span data-stu-id="f37ed-102">Issues with Azure MFA</span></span>
<span data-ttu-id="f37ed-103">Yra keletas dalykų, kuriuos galite patikrinti, jei vartotojai negali prisiregistruoti naudodami kelių dalių autentifikavimą (MFA)</span><span class="sxs-lookup"><span data-stu-id="f37ed-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="f37ed-104">Paveiktą vartotoją galima užblokuoti "Azure Active Directory" portale.</span><span class="sxs-lookup"><span data-stu-id="f37ed-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="f37ed-105">Jei tai yra atvejis, konkretaus vartotojo autentifikavimo bandymai bus automatiškai atmesti.</span><span class="sxs-lookup"><span data-stu-id="f37ed-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="f37ed-106">Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="f37ed-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="f37ed-107">Jei vartotojui neužblokuotas vartotojas arba vartotojas neužblokuotas, galite pabandyti iš naujo nustatyti vartotojo MFA ir jie pereis į registruotis procesą dar kartą.</span><span class="sxs-lookup"><span data-stu-id="f37ed-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="f37ed-108">Atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="f37ed-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="f37ed-109">Jei MFA įgalino pirmą kartą ir jūsų vartotojai negali prisijungti prie naršyklių ne naršyklės, pvz., "Outlook", "Skype" ir kt., galbūt "ADAL" ("Active Directory" autentifikavimo biblioteka) neįgalinta jūsų "O365" prenumeratoje.</span><span class="sxs-lookup"><span data-stu-id="f37ed-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="f37ed-110">Šiuo atveju jums reikės prisijungti prie "Exchange Online" "PowerShell" ir paleisti šį "cmdlet":  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="f37ed-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>