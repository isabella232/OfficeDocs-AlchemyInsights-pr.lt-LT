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
# <a name="api-permissions-and-consent"></a>API teisės ir sutikimas

Programos, kurios integruoja su "Microsoft" tapatybės platforma, pateikia leidimų modelį, kuris leidžia vartotojams ir administratoriams kontroliuoti, kaip galima pasiekti duomenis. Autorizacijos modelio diegimas buvo atnaujintas "Microsoft" tapatybės platformos galinio punkto. Jis pakeis tai, kaip taikomoji programa turi sąveikauti su "Microsoft" tapatybės platforma. ["Microsoft" tapatybės platformos galinio punkto teisės ir sutikimas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) apima pagrindines šio autorizavimo modelio sąvokas, įskaitant aprėptis, teises ir sutikimą.

" [Azure Active Directory" ("AZURE AD") sutikimo sistema](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) leidžia lengvai kurti kelių nuomotojų žiniatinklio ir vietines kliento taikomąsias programas. Šios programos leidžia prisijungti pagal vartotojų paskyras iš "Azure AD" nuomotojo, kuris skiriasi nuo tos vietos, kurioje registruota taikomoji programa. Jiems taip pat gali reikėti prieiti prie žiniatinklio API, pvz., "Microsoft Graph" API (pasiekti "Azure AD", Intune ir "Microsoft" 365) ir kitų "Microsoft" paslaugų API, be savo žiniatinklio API.

