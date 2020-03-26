---
title: Kalendoriaus piktograma nerodo „Teams“ kliento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932201"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendoriaus piktograma nerodo „Teams“ kliento

„Teams“ kalendoriaus skirtukui būtina prieiga prie „Exchange“ pašto dėžutės naudojant „Exchange Web Services“. „Exchange“ pašto dėžutė gali būti internetinė arba vietinė. Interneto vartotojai, kurie nemato kalendoriaus skirtuko, turi įsitikinti, kad jie yra [licencijuoti „Exchange Online“ pašto dėžutei ir pašto dėžutė yra įgalinta](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jei vartotojas turi tinkamą pašto dėžutę „Exchange Online“, tačiau vis tiek nemato kalendoriaus skirtuko, gali būti, kad kilo tinklo problemų. Naudokite [„Microsoft“ nuotolinio ryšio analizatorių](https://testconnectivity.microsoft.com/) ir paveiktam vartotojui atlikite **„Microsoft Exchange“ žiniatinklio tarnybų ryšio testus**.

Galiausiai patikrinkite [„Teams“ programų sąrankos strategijas](https://admin.teams.microsoft.com/policies/app-setup), kad įsitikintumėte, jog kalendoriaus programa nebuvo pašalinta iš vartotojui taikomos strategijos (greičiausiai tai **visuotinis (visos organizacijos numatytasis nustatymas)**.

Jei vartotojai veikia vietoje, būtina įsitikinti, kad hibridinė konfigūracija yra tinkama. Triktims šalinti naudokite [hibridinės konfigūracijos vediklį](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Atkreipkite dėmesį, kad [„Teams“ būtina „Exchange 2016“ CU3 ar naujesnė versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
