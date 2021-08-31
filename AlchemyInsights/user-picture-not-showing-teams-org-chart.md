---
title: Vartotojo paveikslėlis nerodomas Microsoft Teams organizacijos diagramoje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792759"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Vartotojo paveikslėlis nerodomas Microsoft Teams organizacijos diagramoje

Jei vienam ar daugiau organizacijos asmenų organizacijos diagramoje trūksta savo profilio nuotraukos, gali būti, kad **parametras ShowInAddressLists** nustatytas kaip **False**:

1. Eikite "Microsoft 365" administravimo centras > [**aktyvūs vartotojai**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ir pasirinkite vartotoją su trūkstama nuotrauka. 
1. Pasirinkite skirtuką **Paštas** ir įsitikinkite, kad **nustatyta Parinktis** Rodyti visuotiniame adresų **sąraše taip**. 

Jei **parametro ShowInAddressLists** kaip Taip parametras neveikia, patikrinkite šiuos veiksmus: 

- Vartotojas gali būti paslėptas iš gavėjų sąrašo Exchange. Daugiau informacijos žr. [Adresų sąrašų valdymas Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Vartotojas gali būti paslėptas iš adresų sąrašo "Azure Active Directory". Daugiau informacijos žr. ["Set-AzureADUser"](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
