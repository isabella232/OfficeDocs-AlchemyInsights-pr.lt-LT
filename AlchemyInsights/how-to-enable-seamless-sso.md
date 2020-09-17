---
title: Kaip įgalinti sklandžią SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780535"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="0cb20-102">Kaip įgalinti sklandžią SSO</span><span class="sxs-lookup"><span data-stu-id="0cb20-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="0cb20-103">Įgalinkite sklandžią SSO naudodami " [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)".</span><span class="sxs-lookup"><span data-stu-id="0cb20-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="0cb20-104">Jei atliekate naują "Azure AD Connect" diegimą, pasirinkite [pasirinktinio diegimo kelią](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="0cb20-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="0cb20-105">**Vartotojo prisijungimo** puslapyje pasirinkite parinktį **įgalinti bendrąją autentifikacija** .</span><span class="sxs-lookup"><span data-stu-id="0cb20-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="0cb20-106">Norėdami patikrinti, ar tinkamai įjungėte sklandžią SSO:</span><span class="sxs-lookup"><span data-stu-id="0cb20-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="0cb20-107">Prisijunkite prie " [Azure Active Directory" administravimo centro](https://aad.portal.azure.com) kaip visuotinis administratorius.</span><span class="sxs-lookup"><span data-stu-id="0cb20-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="0cb20-108">Kairiojoje srityje pasirinkite " **Azure Active Directory** ".</span><span class="sxs-lookup"><span data-stu-id="0cb20-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="0cb20-109">Patikrinkite, ar **įgalinta**sklandi Bendroji autentifikacija.</span><span class="sxs-lookup"><span data-stu-id="0cb20-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="0cb20-110">Jei norite sužinoti daugiau, peržiūrėkite ["Azure Active Directory" vientisas autentifikacijos: Greitas pasirengimas darbui](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="0cb20-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  