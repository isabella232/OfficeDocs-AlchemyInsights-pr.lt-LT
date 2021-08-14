---
title: Kalendoriaus piktograma nerodo „Teams“ kliento
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989599"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendoriaus piktograma nerodo „Teams“ kliento

„Teams“ kalendoriaus skirtukui būtina prieiga prie „Exchange“ pašto dėžutės naudojant „Exchange Web Services“. „Exchange“ pašto dėžutė gali būti internetinė arba vietinė. Interneto vartotojai, kurie nemato kalendoriaus skirtuko, turi įsitikinti, kad jie yra [licencijuoti „Exchange Online“ pašto dėžutei ir pašto dėžutė yra įgalinta](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jei vartotojas turi tinkamą pašto dėžutę „Exchange Online“, tačiau vis tiek nemato kalendoriaus skirtuko, gali būti, kad kilo tinklo problemų. Naudokite [„Microsoft“ nuotolinio ryšio analizatorių](https://testconnectivity.microsoft.com/) ir paveiktam vartotojui atlikite **„Microsoft Exchange“ žiniatinklio tarnybų ryšio testus**.

Galiausiai patikrinkite [„Teams“ programų sąrankos strategijas](https://admin.teams.microsoft.com/policies/app-setup), kad įsitikintumėte, jog kalendoriaus programa nebuvo pašalinta iš vartotojui taikomos strategijos (greičiausiai tai **visuotinis (visos organizacijos numatytasis nustatymas)**.

Jei vartotojai veikia vietoje, būtina įsitikinti, kad hibridinė konfigūracija yra tinkama. Triktims šalinti naudokite [hibridinės konfigūracijos vediklį](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Atkreipkite dėmesį, kad [„Teams“ būtina „Exchange 2016“ CU3 ar naujesnė versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
