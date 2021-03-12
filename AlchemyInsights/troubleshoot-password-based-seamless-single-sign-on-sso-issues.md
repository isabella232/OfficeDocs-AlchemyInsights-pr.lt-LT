---
title: Nepagrįstų vienkartinio prisijungimo (SSO) problemų sprendimas slaptažodžiu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714880"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="d7f55-102">Nepagrįstų vienkartinio prisijungimo (SSO) problemų sprendimas slaptažodžiu</span><span class="sxs-lookup"><span data-stu-id="d7f55-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="d7f55-103">Jei norite sužinoti, kas yra "SSO" slaptažodį, ieškokite [slaptažodžiu pagrįstas autentifikavimas naudojant "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)".</span><span class="sxs-lookup"><span data-stu-id="d7f55-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="d7f55-104">**SSO pagal slaptažodį konfigūravimas**</span><span class="sxs-lookup"><span data-stu-id="d7f55-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="d7f55-105">[Slaptažodžiu pagrįsto vienkartinio prisijungimo konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – šiame straipsnyje išsamiau apie slaptažodžiu pagrįstą SSO parinktį.</span><span class="sxs-lookup"><span data-stu-id="d7f55-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="d7f55-106">Jei įtrauktai taikomajai programai reikia pasirinktinio konfigūravimo ir turite naudoti SSO pagal slaptažodį, tada šis straipsnis skirtas jums.</span><span class="sxs-lookup"><span data-stu-id="d7f55-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="d7f55-107">[Slaptažodžiu pagrįsto vienkartinio prisijungimo prie "Prem" taikomųjų programų konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – taikomosios programos tarpinis serveris palaiko kelis bendrosios autentifikacijos režimus.</span><span class="sxs-lookup"><span data-stu-id="d7f55-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="d7f55-108">Slaptažodžiu pagrįstas prisijungimas skirtas taikomosioms programoms, kurios naudoja vartotojo vardo ir slaptažodžio derinį autentifikavimui.</span><span class="sxs-lookup"><span data-stu-id="d7f55-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="d7f55-109">Sukonfigūravus slaptažodžiu pagrįstą prisijungimo paraišką, vartotojai turi prisijungti prie vietinio taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="d7f55-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="d7f55-110">Po to, "Azure Active Directory" saugo prisijungimo informaciją ir automatiškai pateikia ją taikomajai programai, kai vartotojai ją pasiekia nuotoliniu būdu.</span><span class="sxs-lookup"><span data-stu-id="d7f55-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="d7f55-111">Jūs jau turite publikuoti ir išbandyti programą naudodami taikomosios programos tarpinį serverį.</span><span class="sxs-lookup"><span data-stu-id="d7f55-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="d7f55-112">Jei ne, atlikite veiksmus [publikuojant taikomąsias programas naudodami "AZURE AD" taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , tada toliau konfigūravimą pagal slaptažodžiu pagrįstą SSO programas.</span><span class="sxs-lookup"><span data-stu-id="d7f55-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="d7f55-113">Jei norite šalinti SSO pagal slaptažodį, žiūrėkite " [Azure AD" bendrosios autentifikacijos "Azure AD" trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="d7f55-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
