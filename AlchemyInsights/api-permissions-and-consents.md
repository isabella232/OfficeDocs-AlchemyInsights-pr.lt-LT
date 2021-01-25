---
title: API teisės ir sutikimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974609"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="55a88-102">API teisės ir sutikimas</span><span class="sxs-lookup"><span data-stu-id="55a88-102">API permissions and consent</span></span>

<span data-ttu-id="55a88-103">Programos, kurios integruoja su "Microsoft" tapatybės platforma, pateikia leidimų modelį, kuris leidžia vartotojams ir administratoriams kontroliuoti, kaip galima pasiekti duomenis.</span><span class="sxs-lookup"><span data-stu-id="55a88-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="55a88-104">Autorizacijos modelio diegimas buvo atnaujintas "Microsoft" tapatybės platformos galinio punkto.</span><span class="sxs-lookup"><span data-stu-id="55a88-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="55a88-105">Jis pakeis tai, kaip taikomoji programa turi sąveikauti su "Microsoft" tapatybės platforma.</span><span class="sxs-lookup"><span data-stu-id="55a88-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="55a88-106">["Microsoft" tapatybės platformos galinio punkto teisės ir sutikimas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) apima pagrindines šio autorizavimo modelio sąvokas, įskaitant aprėptis, teises ir sutikimą.</span><span class="sxs-lookup"><span data-stu-id="55a88-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="55a88-107">" [Azure Active Directory" ("AZURE AD") sutikimo sistema](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) leidžia lengvai kurti kelių nuomotojų žiniatinklio ir vietines kliento taikomąsias programas.</span><span class="sxs-lookup"><span data-stu-id="55a88-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="55a88-108">Šios programos leidžia prisijungti pagal vartotojų paskyras iš "Azure AD" nuomotojo, kuris skiriasi nuo tos vietos, kurioje registruota taikomoji programa.</span><span class="sxs-lookup"><span data-stu-id="55a88-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="55a88-109">Jiems taip pat gali reikėti prieiti prie žiniatinklio API, pvz., "Microsoft Graph" API (pasiekti "Azure AD", Intune ir "Microsoft" 365) ir kitų "Microsoft" paslaugų API, be savo žiniatinklio API.</span><span class="sxs-lookup"><span data-stu-id="55a88-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

