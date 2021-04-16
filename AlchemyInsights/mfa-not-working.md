---
title: MFA problemos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810492"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="404a8-102">"Azure" MFA problemos</span><span class="sxs-lookup"><span data-stu-id="404a8-102">Issues with Azure MFA</span></span>
<span data-ttu-id="404a8-103">Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudodami kelių dalių autentifikavimą (MFA)</span><span class="sxs-lookup"><span data-stu-id="404a8-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="404a8-104">Paveiktas vartotojas gali būti užblokuotas "Azure Active Directory" portale.</span><span class="sxs-lookup"><span data-stu-id="404a8-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="404a8-105">Tokiu atveju autentifikavimo bandymai tam konkrečiam vartotojui bus automatiškai atmesti.</span><span class="sxs-lookup"><span data-stu-id="404a8-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="404a8-106">Atlikite šiame straipsnyje nurodytus veiksmus, kad atblokuokite juos.</span><span class="sxs-lookup"><span data-stu-id="404a8-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="404a8-107">Jei vartotojo blokavimas nepadės arba vartotojas nėra užblokuotas, galite pabandyti iš naujo nustatyti vartotojo MFA ir jis vėl pereis per registracijos procesą.</span><span class="sxs-lookup"><span data-stu-id="404a8-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="404a8-108">Atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="404a8-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="404a8-109">Jei pirmą kartą įgalinote MFA ir jūsų vartotojai negali prisijungti prie ne naršyklių klientų, pvz., "Outlook", "Skype" ir kt., galbūt "ADAL" ("Active Directory" autentifikavimo biblioteka) neįgalinta jūsų "O365" prenumeratoje.</span><span class="sxs-lookup"><span data-stu-id="404a8-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="404a8-110">Tokiu atveju turėsite prisijungti prie "Exchange Online PowerShell" ir paleisti šią "cmdlet":  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="404a8-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>