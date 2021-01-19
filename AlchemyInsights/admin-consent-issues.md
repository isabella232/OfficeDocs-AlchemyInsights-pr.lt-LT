---
title: Administratoriaus sutikimo problemos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901518"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="40eb2-102">Administratoriaus sutikimo problemos</span><span class="sxs-lookup"><span data-stu-id="40eb2-102">Admin consent issues</span></span>

1. <span data-ttu-id="40eb2-103">Įgalinkite [administratoriaus sutikimo darbo eigą](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , kad vartotojai galėtų prašyti Administratoriaus patvirtinimo tiesiogiai iš sutikimo ekrano.</span><span class="sxs-lookup"><span data-stu-id="40eb2-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="40eb2-104">Jei jūs arba jūsų taikomosios programos vartotojai sutikime įvyksta netikėtų klaidų, skaitykite šį straipsnį, kaip atlikti trikčių diagnostikos veiksmus: [netikėta klaida gavus sutikimą su programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="40eb2-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="40eb2-105">Sužinokite daugiau apie [administratoriaus sutikimą "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kaip veikia [sutikimo raginimas](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) ir kaip [įvertinti užklausą dėl nuomotojo masto administratoriaus sutikimo](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="40eb2-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="40eb2-106">Programos, kurios integruoja su "Microsoft" tapatybės platforma, pateikia leidimų modelį, kuris leidžia vartotojams ir administratoriams kontroliuoti, kaip galima pasiekti duomenis.</span><span class="sxs-lookup"><span data-stu-id="40eb2-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="40eb2-107">Autorizacijos modelio diegimas buvo atnaujintas "Microsoft" tapatybės platformos galinio punkto ir pakeičiamas kaip taikomoji programa turi sąveikauti su "Microsoft" tapatybės platforma.</span><span class="sxs-lookup"><span data-stu-id="40eb2-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="40eb2-108">Peržiūrėkite ["Microsoft" tapatybės platformos galinio punkto teises ir sutikimą](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) , kad galėtumėte peržiūrėti šio autorizavimo modelį, įskaitant aprėpčių, teisių ir sutikimo.</span><span class="sxs-lookup"><span data-stu-id="40eb2-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>