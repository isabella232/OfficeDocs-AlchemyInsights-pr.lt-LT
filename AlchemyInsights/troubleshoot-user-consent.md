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
# <a name="troubleshoot-user-consent"></a>Vartotojo sutikimo trikčių šalinimas

1. Galite konfigūruoti, kaip galutiniai vartotojai sutiktų su programomis "Azure" portale arba "PowerShell". Daugiau informacijos ieškokite [vartotojo sutikimo parametruose](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Administratorius taip pat gali naudoti ["Microsoft Graph" API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , kad suteiktų sutikimą perduoti teises vieno vartotojo vardu. Daugiau informacijos ieškokite [vartotojo vardu gauti prieigą](https://docs.microsoft.com/graph/auth-v2-user).
1. [Vartotojo sutikimo klaidos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): šiame straipsnyje aptariamos klaidos, kurios gali įvykti vykstant programos sutikimui. Jei kyla problemų dėl netikėto sutikimo raginimų, kuriuose nėra jokių klaidų žinučių, ieškokite " [AZURE AD" autentifikavimo scenarijai](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).