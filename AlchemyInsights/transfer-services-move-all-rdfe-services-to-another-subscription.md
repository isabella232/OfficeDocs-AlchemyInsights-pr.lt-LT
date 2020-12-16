---
title: Perkėlimo paslaugos – perkelti visas RDFE paslaugas į kitą prenumeratą
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692170"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Perkėlimo paslaugos – perkelti visas RDFE paslaugas į kitą prenumeratą

**Išteklių perkėlimas**

"Azure" išteklius galima perkelti į kitą "Azure" prenumeratą arba išteklių grupę pagal tą pačią prenumeratą, naudojant "Azure" portalą, "Azure PowerShell", "Azure CLI" arba "ILSISI" API išteklių perkėlimą.

Kad galėtumėte perkelti išteklius, žiūrėkite:

- [Kontrolinis sąrašas prieš perkeliant išteklius](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Paslaugos, kurias galima perkelti](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kaip patikrinti perkėlimą](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Paslaugų gairių perkėlimas](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Norėdami perkelti esamus išteklius į kitą išteklių grupę arba prenumeratą, galite naudoti:

- ["Azure" portalas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- ["Azure PowerShell"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- ["Azure CLI"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- ["POILSIU API"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Vadovėlis: " [Azure" išteklių perkėlimas į kitą išteklių grupę arba prenumeratą](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Klaidų šalinimas naudojant "Azure Resource Manager"**

Skaitykite toliau pateiktus straipsnius, Norėdami sužinoti apie kai kurias įprastas "Azure" diegimo klaidas ir gauti informaciją, kad jas išspręstumėte. Jei nerandate diegimo klaidos klaidos kodo, žiūrėkite [rasti klaidos kodą](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Diegimo klaidų šalinimas](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- ["Azure" išteklių perkėlimo į naują išteklių grupę arba prenumeratą trikčių šalinimas](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Nepamirškite, kad jei norite atnaujinti savo "Azure" prenumeratą, pvz., pereiti nuo nemokamos iki apmokėjimo, turėsite konvertuoti prenumeratą.

- Jei norite atnaujinti nemokamą bandomąją versiją, peržiūrėkite [nemokamą bandomąją versiją arba "Microsoft" Įsivaizduokite "Azure" prenumeratą, kad galėtumėte sumokėti](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Norėdami pakeisti "Pay-as-you-go" paskyrą, skaitykite " [Azure Pay-as-you-go" prenumeratos keitimas kitu pasiūlymu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Norėdami įtraukti arba susieti "Azure" prenumeratą į "Azure Active Directory" nuomotoją:**

1. Prisijunkite ir pasirinkite prenumeratą, kurią norite naudoti " [Azure" portalo puslapyje prenumeratos](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Pasirinkite **keisti katalogą**.
3. Peržiūrėkite visus rodomus įspėjimus ir pasirinkite **keisti**.
4. Šis katalogas pakeičiamas į prenumeratą ir gausite pranešimą apie sėkmę.
5. Naudokite *katalogo* jungiklį, kad pereitumėte į naują katalogą. Gali užtrukti iki 10 minučių, kol viskas rodoma tinkamai.

**Rekomenduojami dokumentai**

- ["Azure" prenumeratos nuosavybės perdavimas](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Išteklių perkėlimas į naują išteklių grupę arba prenumeratą](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Išteklių valdymas naudojant "Azure" portalą](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
