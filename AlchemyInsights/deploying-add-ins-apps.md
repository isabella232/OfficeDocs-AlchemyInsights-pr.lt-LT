---
title: "\"\"Microsoft 365\" programos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125678"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>""Microsoft 365" programos

Centralizuotas diegimas yra rekomenduojamas būdas diegti Office papildinių vartotojams ir grupėms jūsų organizacijoje. Norėdami įdiegti papildiniai, atlikite toliau nurodytus veiksmus.

**Pastaba:** Norėdami įdiegti papildinių, Office kaip atskiras vartotojas, žr. Papildinių rodymas, valdymas [ir diegimas Office programose.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Taip pat įsitikinkite, kad įgalintas Office parduotuvės papildinių įsigijimas. 

1. Įsitikinkite, kad jūsų aplinka atitinka papildinių diegimo naudojant centralizuotą diegimą reikalavimus. Daugiau informacijos žr. [Reikalavimai](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Eikite **Parametrai** Integruotos programos Gaukite programėlių  >    >   Microsoft 365 administravimo centre, kad diegdami papildiniai. 

Pastabos: 

- Integruotos programos reikalauja, kad administratorius turėtų visuotinio administratoriaus arba Exchange administratoriaus teises.

- Kai papildiniai diegiami keliems vartotojams, rekomenduojame užduotis atlikti naudojant grupes, o ne atskirus vartotojus. Daugiau informacijos [žr. Papildinių priskyrimo vartotojams ir grupėms aspektai.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizuotas diegimas nepalaiko vartotojų įdėtosiose grupėse arba grupėse, kurios turi pirmines grupes. Daugiau informacijos [žr. Vartotojų ir grupių užduotys](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Įsitikinkite, kad "Microsoft 365 App Management Service" (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') yra įgalinta vartotojams prisijungti. Daugiau informacijos žr. [Taikomosios programos ypatybės konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Jei kyla problemų diegiant papildinį naudojant integruotas programas, pabandykite įdiegti naudodami [papildinį.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Daugiau informacijos rasite:

[Papildiniai diegiami administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Papildiniai administravimo centre](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Centralizuoto diegimo "PowerShell" "cmdlet" naudojimas papildinių valdymas](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publikavimas Office papildiniai naudojant centralizuotą diegimą Microsoft 365 administravimo centre](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Trikčių šalinimas: vartotojas nematote papildiniai](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Vartotojo klaidų šalinimas naudojant Office papildiniai](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)