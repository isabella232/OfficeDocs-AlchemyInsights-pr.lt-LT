---
title: Klasikinės "SharePoint" audito žurnalų ataskaitos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662216"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>"SharePoint" ir "OneDrive" audito žurnalai

## <a name="sharepoint-classic-audit-logs"></a>"SharePoint Classic" audito žurnalai

SPO senstelėjusios įrangos tikrinimas perkeltas į bendrąjį audito (UAL) pranešimą. Visos SPO senstelėjusios audito ataskaitos dabar bus perkeltos į UAL, o senstelėjusių audito signalai perkelti į UAL.

Pagrindiniai pokyčiai:

* Apipjaustymas negalimas kaip pajėgumas.
* NEGALIMA pasirinkti konkrečių įvykių audito. [Šiame dokumente](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) rasite išsamų pagal numatytuosius numatytuosius tikrinamų įvykių sąrašą.
* Parinkties **vieta** dalyje **tinkintos ataskaitos** nėra.
* NEGALIMA naudoti parinkties **atidaryti arba atsisiųsti dokumentų** įvykių.

[Svetainių rinkinio audito parametrų konfigūravimas](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>"SharePoint" ir "OneDrive" modernūs suvienodinti audito žurnalai iš atitikties

* [Vieningosios audito žurnalų įjungimas/išjungimas](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

"SharePoint" arba "OneDrive" nereikia jokių papildomų konfigūracijų.

Audito žurnalų ieškos naudojimas norint patikrinti failo (-ų), aplanko (-ų), vartotojo (-ų), teisių:

* [Failų ir puslapių veikla](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aplanko veikla](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Naudojimo ir prieigos užklausų veikla](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Sinchronizavimo veikla](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Svetainės administravimo veikla](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Daugiau informacijos apie tai, kaip gauti šiuos įvykius, ieškokite [audito žurnalų ieška](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
