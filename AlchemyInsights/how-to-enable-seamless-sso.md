---
title: Kaip įjungti sklandžią SSO
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825739"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="4d1fe-102">Kaip įjungti sklandžią SSO</span><span class="sxs-lookup"><span data-stu-id="4d1fe-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="4d1fe-103">Įjunkite sklandų SSO per ["Azure AD Connect".](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="4d1fe-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="4d1fe-104">Jei atliekate naują "Azure AD Connect" diegimą, pasirinkite [pasirinktinį diegimo kelią](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="4d1fe-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="4d1fe-105">Puslapyje **Vartotojo prisijungimas pasirinkite** parinktį Įgalinti **bendrąją a prisijungimą.**</span><span class="sxs-lookup"><span data-stu-id="4d1fe-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="4d1fe-106">Norėdami patikrinti, ar tinkamai įgalinote sklandžią SSO:</span><span class="sxs-lookup"><span data-stu-id="4d1fe-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="4d1fe-107">Prisijunkite prie ["Azure Active Directory" administravimo centro kaip](https://aad.portal.azure.com) visuotinis administratorius.</span><span class="sxs-lookup"><span data-stu-id="4d1fe-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="4d1fe-108">Kairiojoje **srityje pasirinkite "Azure Active Directory".**</span><span class="sxs-lookup"><span data-stu-id="4d1fe-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="4d1fe-109">Patikrinkite, ar vientisa bendroji a prisijungimo funkcija **įgalinta**.</span><span class="sxs-lookup"><span data-stu-id="4d1fe-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="4d1fe-110">Norėdami sužinoti daugiau, žr. ["Azure Active Directory Seamless Single Sign-On": greitas paleidimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="4d1fe-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  