---
title: API teisių ir sutikimo procesas
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404874"
---
# <a name="api-permissions-and-consent-process"></a>API teisių ir sutikimo procesas

Kad jūsų programa turėtų prieigą prie "Microsoft Graph" duomenų, vartotojas arba administratorius turi suteikti jai reikiamas teises per sutikimo procesą. ["Microsoft Graph" teisių](https://docs.microsoft.com/graph/permissions-reference) nuorodoje išvardytos teisės, susietos su kiekvienu dideliu "Microsoft Graph" API komplektu. Jame taip pat pateikiama patarimų, kaip naudoti teises.

**Nustatyti arba atnaujinti pagrindinę tarnybos paslaugą**

- [Kurti "serviceprincipal"](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – šiame straipsnyje rodoma, kaip sukurti naują "servicePrincipal" objektą.
- [Sukurkite "Azure AD" &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) pagrindinę tarnybą portale – šiame straipsnyje rodoma, kaip sukurti naują "Azure Active Directory" ("Azure AD") taikomąją programą ir tarnybos pagrindinę programą, kurią galima naudoti su vaidmenimis pagrįstu prieigos valdikliu.
- [Programos & "Azure AD"](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – šiame straipsnyje aprašoma taikomosios programos registracija, taikomosios programos objektai ir tarnybos principai "Azure Active Directory": kas jie yra, kaip jie naudojami ir kaip jie yra susiję vienas su kitu.

**Įtraukite arba atnaujinkite taikomosios programos registraciją ir pateikite administratoriaus sutikimą**

- [Taikomosios programos registracijos kūrimas](https://docs.microsoft.com/graph/api/application-post-applications) – šiame straipsnyje rodoma, kaip sukurti naują programos objektą.
- [Taikomosios programos registracijos naujinimas – API](https://docs.microsoft.com/graph/api/application-update) teisės – šiame straipsnyje rodoma, kaip atnaujinti programos objekto ypatybes.
- [Pateikite administratoriaus](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) sutikimą – norėdami gauti administratoriaus sutikimą ir sutikimą apskritai, reikalaujame, kad administratorius aiškiai dės sutikimą.
- [RBAC (beta versija)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – "Microsoft 365 RBAC" teikėjų vaidmenų valdymo konteineris, skirtas vieningoms vaidmenų apibrėžtims ir vaidmenų užduotims, kurios palaiko kelias pagrindines ir kelias aprėptis vienoje vaidmenų užduočiai. Tai skiriasi nuo *"rbacApplication"* ištekliaus tipo. "Microsoft Intune" yra tokio RBAC teikėjo pavyzdys. Vaidmenų priskyrimas "Intune" gali turėti pagrindinių elementų masyvą ir aprėpties grupių masyvą. **Tai yra beta versija, tai reiškia, kad ji vis dar yra besivysto ir nerekomenduojama naudoti gamybai.**
