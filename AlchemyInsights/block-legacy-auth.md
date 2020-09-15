---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685606"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="e0ecf-102">Senstelėjusio autentifikavimo blokavimas</span><span class="sxs-lookup"><span data-stu-id="e0ecf-102">Blocking legacy authentication</span></span>

<span data-ttu-id="e0ecf-103">Senstelėjęs autentifikavimas yra terminas, nurodantis autentifikavimo užklausą, kurią pateikia:</span><span class="sxs-lookup"><span data-stu-id="e0ecf-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="e0ecf-104">Senesni "Office" Klientai, naudojantys šiuolaikinį autentifikavimą (pvz., "Office 2010" klientą).</span><span class="sxs-lookup"><span data-stu-id="e0ecf-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="e0ecf-105">Bet kuris klientas, kuris naudoja senstelėjusius pašto protokolus, pvz., IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="e0ecf-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="e0ecf-106">Daugiau informacijos apie senstelėjusio autentifikavimo blokavimą ir modernaus autentifikavimo įgalinimą rasite [senstelėjusio autentifikavimo blokavimą](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="e0ecf-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="e0ecf-107">"Azure Active Directory" numatytoji saugos reikšmė ("Azure AD") padeda apsaugoti jūsų organizaciją ir ją apsaugoti.</span><span class="sxs-lookup"><span data-stu-id="e0ecf-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="e0ecf-108">Saugos numatytose yra iš anksto sukonfigūruoti bendrųjų atakų saugos parametrai.</span><span class="sxs-lookup"><span data-stu-id="e0ecf-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="e0ecf-109">Daugiau informacijos apie saugos numatytąsias reikšmes rasite [kas yra saugos numatytosios reikšmės?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="e0ecf-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="e0ecf-110">**Pastaba**: jei jūsų nuomotojas buvo sukurtas arba po spalio 22 d., "2019", gali būti, kad kyla naujų saugių pagal numatytuosius parametrus ir jūsų nuomotojuje jau yra įgalintos saugos numatytosios reikšmės.</span><span class="sxs-lookup"><span data-stu-id="e0ecf-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="e0ecf-111">Siekiant apsaugoti visus vartotojus, numatytosios saugos reikšmės yra diegiamos visiems naujiems nuomininkams, sukurtiems.</span><span class="sxs-lookup"><span data-stu-id="e0ecf-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
