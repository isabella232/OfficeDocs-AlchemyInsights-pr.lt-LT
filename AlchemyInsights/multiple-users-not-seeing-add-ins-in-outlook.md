---
title: Keli vartotojai nemato papildinių "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197979"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Keli vartotojai nemato papildinių "Outlook"

Jei išbandysite "Outlook" papildinius ir nė vienas rodomas, kaip pirmą trikčių šalinimo veiksmą, naudokite **Get-OrganizationConfig** "PowerShell" cmdlet pateikti užklausą _AppsForOfficeEnabled_ parametras. Jei užklausa grąžina **reikšmę false**, nustatykite šį parametrą **true** naudojant **Set-OrganizationConfig** cmdlet, todėl priedai rodomi kaip tikėtasi.

Nerekomenduojame, kad _Parametras AppsForOfficeEnabled_ nustatytas kaip **Klaidingas**. **Reikšmė False** panaikina visus anksčiau nurodytus administravimo ir vartotojo vaidmens parametrus ir neleidžia bet kuriam organizacijos vartotojui suaktyvinti naujų programų.

Daugiau informacijos [ieškokite Administratorių ir vartotojų, kurie gali įdiegti ir tvarkyti "Outlook" papildinius, nurodymas.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)