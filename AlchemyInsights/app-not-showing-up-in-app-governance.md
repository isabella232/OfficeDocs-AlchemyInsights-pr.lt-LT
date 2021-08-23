---
title: Programėlė nerodoma programų valdyme
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454694"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Programėlė nerodoma programų valdyme

Jei jūsų taikomoji programa nerodoma programų valdyme, patikrinkite šiuos veiksmus:

1. Eikite [į "Azure AD"](https://aad.portal.azure.com/) ir raskite taikomosios programos ID puslapio Apžvalga viršutinėje juostoje ieškodami taikomosios programos pavadinimo.

1. "Access "Graph" Explorer" ir ieškokite taikomosios programos ID savo paslaugoje, naudodami šią užklausą ir pakeisdami atitinkamą taikomosios programos <appId> ID: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Jei nepateikiami jokie rezultatai, ieškokite taikomosios programos ID naudodami šią užklausą ir pakeisdami atitinkamą taikomosios programos <appId> ID: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Jei kyla problemų dėl užklausos, žr. [Palaikymo gaukite](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Daugiau informacijos arba įžvalgų apie programėles programų valdyme [žr. Sužinokite apie matomumą ir įžvalgas.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Daugiau informacijos apie programėlių peržiūrą žr. [Programėlių peržiūra](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
