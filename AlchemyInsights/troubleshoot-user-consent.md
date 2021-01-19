---
title: Vartotojo sutikimo trikčių šalinimas
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901623"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="d18f5-102">Vartotojo sutikimo trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="d18f5-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="d18f5-103">Galite konfigūruoti, kaip galutiniai vartotojai sutiktų su programomis "Azure" portale arba "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="d18f5-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="d18f5-104">Daugiau informacijos ieškokite [vartotojo sutikimo parametruose](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="d18f5-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="d18f5-105">Administratorius taip pat gali naudoti ["Microsoft Graph" API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , kad suteiktų sutikimą perduoti teises vieno vartotojo vardu.</span><span class="sxs-lookup"><span data-stu-id="d18f5-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="d18f5-106">Daugiau informacijos ieškokite [vartotojo vardu gauti prieigą](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="d18f5-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="d18f5-107">[Vartotojo sutikimo klaidos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): šiame straipsnyje aptariamos klaidos, kurios gali įvykti vykstant programos sutikimui.</span><span class="sxs-lookup"><span data-stu-id="d18f5-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="d18f5-108">Jei kyla problemų dėl netikėto sutikimo raginimų, kuriuose nėra jokių klaidų žinučių, ieškokite " [AZURE AD" autentifikavimo scenarijai](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="d18f5-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>