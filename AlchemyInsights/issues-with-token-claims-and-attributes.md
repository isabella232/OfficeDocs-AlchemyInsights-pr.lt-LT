---
title: Su atpažinimo ženklų reikalavimais ir atributais susijusios problemos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035966"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="b8f79-102">Su atpažinimo ženklų reikalavimais ir atributais susijusios problemos</span><span class="sxs-lookup"><span data-stu-id="b8f79-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="b8f79-103">**Atpažinimo ženklų reikalavimų naujinimas, konfigūravimas arba šalinimas**</span><span class="sxs-lookup"><span data-stu-id="b8f79-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="b8f79-104">Naudodami "Azure Active Directory" ("Azure AD"), atsakymų atpažinimo ženkle, kurį gaunate po to, kai įgaliojate taikomąją programą, galite [Tinkinti vaidmens reikalavimo tipą](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) .</span><span class="sxs-lookup"><span data-stu-id="b8f79-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="b8f79-105">Taikomųjų programų kūrėjai savo "Azure AD" taikomosiose programose gali naudoti pasirinktines pretenzijas, kad nurodytų, kokius teiginius jie nori naudoti žetonams, siunčiamiems į jų taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="b8f79-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="b8f79-106">Daugiau informacijos ieškokite [pasirinktinių reikalavimų pateikimas programėlei](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="b8f79-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="b8f79-107">[Konfigūruokite "Azure Active Directory" taikomųjų programų grupės reikalavimus](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="b8f79-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="b8f79-108">Jei naudojate sklandžią bendrąją autentifikacijos programą, žiūrėkite [Tinkinti reikalavimus, pateiktus "SAML" atpažinimo ženklo įmonėms taikomosiose programose](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="b8f79-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="b8f79-109">**Atributų atributo susiejimas**</span><span class="sxs-lookup"><span data-stu-id="b8f79-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="b8f79-110">Norėdami konfigūruoti pretenzijų atvaizdavimo strategiją naudodami "PowerShell", žiūrėkite [Tinkinti teiginius, pateiktus "Tokens" konkrečios programos nuomotojuje (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="b8f79-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="b8f79-111">Katalogo schemos plėtinio atributai – tai būdas saugoti papildomus duomenis "Azure Active Directory" vartotojo objektams ir kitiems katalogo objektams, pvz., grupėms, nuomotojo duomenims, paslaugų direktams.</span><span class="sxs-lookup"><span data-stu-id="b8f79-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="b8f79-112">Galima naudoti tik plėtinio atributus vartotojo objektuose.</span><span class="sxs-lookup"><span data-stu-id="b8f79-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="b8f79-113">[Naudojant katalogų schemos plėtinio atributus teiginiams](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) nurodoma, kaip naudoti katalogo schemos plėtinio atributus siunčiant vartotojo duomenis į taikomąsias programas atpažinimo ženklų ieškiniams.</span><span class="sxs-lookup"><span data-stu-id="b8f79-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="b8f79-114">Daugiau informacijos apie simbolinius teiginius rasite:</span><span class="sxs-lookup"><span data-stu-id="b8f79-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="b8f79-115">"Access" atpažinimo ženklų pretenzijos</span><span class="sxs-lookup"><span data-stu-id="b8f79-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="b8f79-116">Ieškiniai id_token</span><span class="sxs-lookup"><span data-stu-id="b8f79-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="b8f79-117">[Teigia](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , kad galite tikėtis ID atpažinimo ženklai ir prieigos žetonai, kuriuos išleido "Azure AD" B2C</span><span class="sxs-lookup"><span data-stu-id="b8f79-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="b8f79-118">SAML atpažinimo ženklo pretenzijų nuoroda</span><span class="sxs-lookup"><span data-stu-id="b8f79-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
