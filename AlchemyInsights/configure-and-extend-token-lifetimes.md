---
title: Simbolinis gyvenimo trukmės konfigūravimas ir išplėtimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917005"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="23df1-102">Simbolinis gyvenimo trukmės konfigūravimas ir išplėtimas</span><span class="sxs-lookup"><span data-stu-id="23df1-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="23df1-103">Galite apibrėžti "Microsoft" tapatybės platformos išduoto prieigos, SAML arba ID atpažinimo ženklo galiojimo laiką.</span><span class="sxs-lookup"><span data-stu-id="23df1-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="23df1-104">Galite nustatyti atpažinimo ženklų naudojimo visas savo organizacijos taikomąsias programas, kelių nuomotojų (kelių organizacijų) taikomąją programą arba konkrečią organizacijos pagrindinę tarnybą.</span><span class="sxs-lookup"><span data-stu-id="23df1-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="23df1-105">Daugiau informacijos rasite [konfigūruotinas atpažinimo ženklų naudojimo laikas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="23df1-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="23df1-106">Pavyzdžiuose rasite [pavyzdžių, kaip sukonfigūruoti atpažinimo ženklų naudojimo laiką](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="23df1-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="23df1-107">Norėdami sužinoti, kaip sukonfigūruoti atpažinimo ženklo gyvavimo laiką ir suderinamumą "Azure Active Directory" B2C ("Azure AD B2C"), žiūrėkite " [Azure Active Directory" "B2C" esančių atpažinimo ženklų konfigūravimas](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="23df1-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="23df1-108">Straipsnyje [Konfigūruokite seanso veikimą "Azure Active Directory](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) " "B2C" aprašomi bendrosios AUTENTIFIKACIJOS (SSO) metodai, naudojami "AZURE ad B2C", ir padeda pasirinkti tinkamiausią SSO metodą konfigūruojant savo strategiją.</span><span class="sxs-lookup"><span data-stu-id="23df1-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="23df1-109">**Kiek laiko žetonai trunka? Kiek laiko galioja?**</span><span class="sxs-lookup"><span data-stu-id="23df1-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="23df1-110">Atpažinimo ženklų naudojimo laikas yra 1 valanda, o seanso trukmė – 24 valandos.</span><span class="sxs-lookup"><span data-stu-id="23df1-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="23df1-111">Tai reiškia, kad jei per 24 valandas nebuvo pateikta jokių prašymų, prieš prašydami naujo atpažinimo ženklo turėsite vėl prisiregistruoti.</span><span class="sxs-lookup"><span data-stu-id="23df1-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="23df1-112">2020 gegužės 30 d., "", joks naujas nuomotojas negalės naudoti Konfigūruotinos atpažinimo ženklo naudojimo strategijos, kad sukonfigūruotumėte seansą ir atnaujintų žetonų.</span><span class="sxs-lookup"><span data-stu-id="23df1-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="23df1-113">Nuteistųjų bus įvykti per kelis mėnesius po to, o tai reiškia, kad mes sustabdysime esamą seansą ir atnaujinsime žetonų politikos kryptis.</span><span class="sxs-lookup"><span data-stu-id="23df1-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="23df1-114">Vis dar galite sukonfigūruoti prieigos atpažinimo ženklo naudojimo laiką po nuteistųjų.</span><span class="sxs-lookup"><span data-stu-id="23df1-114">You can still configure access token lifetimes after the deprecation.</span></span>






