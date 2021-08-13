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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007906"
---
# <a name="troubleshoot-user-consent"></a>Vartotojo sutikimo trikčių šalinimas

1. Galite konfigūruoti, kaip galutiniai vartotojai sutinka su programomis per "Azure" portalą arba "PowerShell". Daugiau [informacijos žr. Vartotojo](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) sutikimo parametrai.
1. Administratorius taip pat gali naudoti ["Microsoft "Graph" API,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) kad duotų sutikimą suteikti įgaliotas teises vieno vartotojo vardu. Daugiau informacijos [žr. Prieiga vartotojo vardu.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Vartotojo sutikimo klaidos:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)šiame straipsnyje aptariamos klaidos, kurios gali įvykti sutikimo su programa proceso metu. Jei šalinant netikėtų sutikimo raginimų, kuriuose nėra klaidų pranešimų, trikčių diagnostiką, žr. ["Azure AD" autentifikavimo scenarijai.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)