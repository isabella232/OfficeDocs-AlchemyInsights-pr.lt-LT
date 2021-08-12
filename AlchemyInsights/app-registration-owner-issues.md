---
title: Taikomosios programos registracijos savininko problemos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951141"
---
# <a name="app-registration-owner-issues"></a>Taikomosios programos registracijos savininko problemos

Toliau pateikiami galimi būdai įtraukti vadovus kaip taikomųjų programų registracijų savininkus:

- "Azure AD PowerShell" modulio naudojimas –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Nuoroda: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- "Azure CLI" naudojimas – `az ad app owner add`

    Nuoroda: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS "Graph" -

    Nuoroda: [Įtraukti savininką – "Microsoft "Graph" v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- "Azure AD" portalo naudojimas – pereikite [į portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners

**Negalite peržiūrėti savo taikomosios programos "App Registrations" ašmenyje, net jei esate tos taikomosios programos savininkas?**

Taikomosios programos savininkas nėra administravimo vaidmuo. Jei parametras [Apriboti prieigą prie "Azure AD"](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) administravimo portalo įgalintas, tada tik administratorius galės peržiūrėti taikomąsias programas taikomųjų programų registracijos portale. Kad savininkas galėtų peržiūrėti taikomąsias programas, išjunkite šį parametrą (nustatykite jį kaip NE) arba priskirkite savininkui tik konkrečios taikomosios programos administratoriaus vaidmenį. Tačiau tam reikės "Azure AD Premium P2" licencijos ir įgalinti ["Privileged Identity Management"](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
