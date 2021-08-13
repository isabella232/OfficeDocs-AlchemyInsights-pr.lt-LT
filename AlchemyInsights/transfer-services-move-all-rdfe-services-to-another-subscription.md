---
title: Perkėlimo paslaugos – perkelkite visas RDFE tarnybas į kitą prenumeratą
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940072"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Perkėlimo paslaugos – perkelkite visas RDFE tarnybas į kitą prenumeratą

**Išteklių perkėlimas**

"Azure" išteklius galima perkelti į kitą "Azure" prenumeratą arba išteklių grupę pagal tą pačią prenumeratą naudojant "Azure" portalą, "Azure PowerShell", "Azure CLI" arba REST API, kad perkeltų išteklius.

Prieš perkeliant išteklius, žr.:

- [Kontrolinis sąrašas prieš perkeliant išteklius](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Paslaugos, kurias galima perkelti](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kaip patikrinti ėjimas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Tarnybų nurodymų perkėlimas](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Norėdami perkelti esamus išteklius į kitą išteklių grupę arba prenumeratą, galite naudoti:

- ["Azure" portalas](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- ["Azure PowerShell"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- ["Azure CLI"](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Mokymo priemonė: ["Azure" išteklių perkėlimas į kitą išteklių grupę arba prenumeratą](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Trikčių šalinimas naudojant "Azure Resource Manager"**

Peržiūrėkite toliau pateikiamus straipsnius, kad sužinotumėte apie kai kurias įprastas "Azure" diegimo klaidas ir gaukite informaciją, kad jas išspręstumėte. Jei nerandate diegimo klaidos kodo, žr. [Klaidos kodo radus](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Diegimo klaidų trikčių šalinimas](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- ["Azure" išteklių perkėlimas į naują išteklių grupę arba prenumeratą trikčių šalinimas](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Atminkite, kad jei norite atnaujinti "Azure" prenumeratą, pvz., pereiti nuo nemokamos prie mokamo, turėsite konvertuoti prenumeratą.

- Norėdami atnaujinti nemokamą bandomąją versiją, žr. Nemokamos bandomosios versijos versijos naujinimas arba ["Microsoft Imagine Azure" prenumerata į "Pay-As-You-Go".](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Norėdami pakeisti "Pay-as-you-go" paskyrą, žr. ["Azure Pay-As-You-Go" prenumeratos](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)keitimas į kitą pasiūlymą.

**Norėdami įtraukti arba susieti "Azure" prenumeratą su "Azure Active Directory" nuomotoju:**

1. Prisijunkite ir pasirinkite norimą naudoti prenumeratą ["Azure" portalo puslapyje Prenumeratos.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Pasirinkite **Keisti katalogą**.
3. Peržiūrėkite visus rodomi įspėjimus, tada pasirinkite **Keisti**.
4. Prenumeratos katalogas pakeičiamas ir gausite sėkmingą pranešimą.
5. Norėdami pereiti *į* naują katalogą, naudokite katalogų perjungiklį. Gali užtrukti iki 10 minučių, kol viskas bus rodoma tinkamai.

**Rekomenduojami dokumentai**

- ["Azure" prenumeratos nuosavybės perdavimas](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Perkelti išteklius į naują išteklių grupę arba prenumeratą](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Išteklių valdymas naudojant "Azure" portalą](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
