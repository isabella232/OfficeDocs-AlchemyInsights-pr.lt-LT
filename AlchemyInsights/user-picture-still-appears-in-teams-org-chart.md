---
title: Vartotojo paveikslėlis vis dar rodomas Microsoft Teams organizacijos diagramoje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422249"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Vartotojo paveikslėlis vis dar rodomas Microsoft Teams organizacijos diagramoje

Jei vienas ar daugiau organizacijos asmenų buvo išjungti arba pašalinti, o jų profilio nuotrauka vis dar rodoma organizacijos diagramoje, gali būti, kad **parametras ShowInAddressLists** nustatytas kaip False: 

1. Eikite "Microsoft 365" administravimo centras > [aktyvūs vartotojai](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) ir pasirinkite vartotoją su vis dar rodoma nuotrauka. 
1. Pasirinkite skirtuką **Paštas** ir įsitikinkite, kad **nustatyta** Parinktis Rodyti visuotiniame adresų **sąraše ne**.

Jei **parametro ShowInAddressLists** kaip **Ne** parametras neveikia, patikrinkite šiuos veiksmus: 

- Vartotojas gali būti rodomas iš gavėjų sąrašo Exchange. Daugiau informacijos žr. [Adresų sąrašų tvarkymas](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)Exchange Online . 
- Vartotojas gali būti rodomas iš adresų sąrašo "Azure Active Directory". Daugiau informacijos žr. ["Set-AzureADUser"](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 