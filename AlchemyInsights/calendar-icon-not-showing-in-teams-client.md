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
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819961"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendoriaus piktograma nerodo „Teams“ kliento

„Teams“ kalendoriaus skirtukui būtina prieiga prie „Exchange“ pašto dėžutės naudojant „Exchange Web Services“. „Exchange“ pašto dėžutė gali būti internetinė arba vietinė. Interneto vartotojai, kurie nemato kalendoriaus skirtuko, turi įsitikinti, kad jie yra [licencijuoti „Exchange Online“ pašto dėžutei ir pašto dėžutė yra įgalinta](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jei vartotojas turi tinkamą pašto dėžutę „Exchange Online“, tačiau vis tiek nemato kalendoriaus skirtuko, gali būti, kad kilo tinklo problemų. Naudokite [„Microsoft“ nuotolinio ryšio analizatorių](https://testconnectivity.microsoft.com/) ir paveiktam vartotojui atlikite **„Microsoft Exchange“ žiniatinklio tarnybų ryšio testus**.

Galiausiai patikrinkite [„Teams“ programų sąrankos strategijas](https://admin.teams.microsoft.com/policies/app-setup), kad įsitikintumėte, jog kalendoriaus programa nebuvo pašalinta iš vartotojui taikomos strategijos (greičiausiai tai **visuotinis (visos organizacijos numatytasis nustatymas)**.

Jei vartotojai veikia vietoje, būtina įsitikinti, kad hibridinė konfigūracija yra tinkama. Triktims šalinti naudokite [hibridinės konfigūracijos vediklį](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Atkreipkite dėmesį, kad [„Teams“ būtina „Exchange 2016“ CU3 ar naujesnė versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
