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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768845"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="5cb0d-102">Problemos su Azure MFP</span><span class="sxs-lookup"><span data-stu-id="5cb0d-102">Issues with Azure MFA</span></span>
<span data-ttu-id="5cb0d-103">Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudojant kelių dalių autentifikavimas (DTS)</span><span class="sxs-lookup"><span data-stu-id="5cb0d-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="5cb0d-104">Susijusio vartotojo gali būti užblokuotas Azure Active Directory portale.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="5cb0d-105">Tokiu atveju autentifikavimas bando, kad konkretus vartotojas bus automatiškai atmestas.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="5cb0d-106">Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="5cb0d-107">Jei atblokavimo vartotojas nepadėjo arba vartotojas nėra užblokuotas galite pabandyti iš naujo MFP vartotojo ir jie bus eiti per Registruotis procesas dar kartą.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="5cb0d-108">Atlikite šiame straipsnyje nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="5cb0d-109">Jei tai pirmas kartas, kai įjungėte DTS ir jūsų vartotojai negali prisijungti prie ne naršyklės klientams, pvz., "Outlook", "Skype" ir tt, galbūt Alma (Active Directory autentifikavimo biblioteka) neįgalintas jūsų O365 prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="5cb0d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="5cb0d-110">Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir paleisti šį cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="5cb0d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>