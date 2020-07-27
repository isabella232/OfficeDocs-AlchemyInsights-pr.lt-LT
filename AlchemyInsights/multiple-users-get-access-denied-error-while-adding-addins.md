---
title: Keli vartotojai gauna "Access Denied" klaidą, kai pridedate papildinius programoje "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424168"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Keli vartotojai gauna "Access Denied" klaidą, kai pridedate papildinius programoje "Outlook"

Galite nurodyti, kurie jūsų organizacijos administratoriai turi teisę diegti ir tvarkyti "Outlook" priedus. Taip pat galite nurodyti, kurie jūsų organizacijos vartotojai turi teisę diegti ir valdyti priedus savo reikmėms.

Daugiau informacijos [ieškokite Administratorių ir vartotojų, kurie gali įdiegti ir tvarkyti "Outlook" papildinius, nurodymas.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)

Norėdami patikrinti, ar sėkmingai priskyrėte vartotojo teises, pakeiskite <Role Name> vaidmens, kurį norite patikrinti, pavadinimu ir vykdykite šią komandą "Exchange Online PowerShell":

Get-ManagementRoleAssignment -Vaidmuo <Role Name> " " -GetEffectiveUsers

Šiame pavyzdyje parodyta, kaip patikrinti, kam priskyrėte teises diegti priedus iš organizacijos "Office" parduotuvės.

Powershell

-Vaidmuo "Org Marketplace Apps" -GetEffectiveUsers

Rezultatuose, Get-ManagementRoleAssignment, peržiūrėkite įrašus efektyvus vartotojai stulpelyje.

Išsamesnės sintaksės ir parametrų informacijos ieškokite [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 