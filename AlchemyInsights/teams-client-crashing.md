---
title: Genda „Teams“ klientas?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030680"
---
# <a name="teams-client-crashing"></a>Genda „Teams“ klientas?

Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:

- Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Įsitikinkite, kad visi [„Office 365“ URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) pasiekiami.

- Prisijunkite naudodami savo administratoriaus paskyrą ir patikrinkite [tarnybų sveikatos stebėjimo skydą](https://docs.microsoft.com/office365/enterprise/view-service-health), kad įsitikintumėte, jog nėra trikčių ar tarnybos veikimo pablogėjimo.

 - Paskutinis veiksmas, kurį galite atlikti – pabandyti išvalyti savo „Teams“ kliento talpyklą:

    1.  Visiškai išeikite iš „Microsoft Teams“ kompiuterio kliento. Galite dešiniuoju pelės mygtuku spustelėti **„Teams“** piktogramų dėkle ir spustelėti **Uždaryti** arba galite paleisti užduočių tvarkytuvą ir visiškai nutraukti procesą.

    2.  Eikite į failų naršyklę ir įveskite %appdata%\Microsoft\teams.

    3.  Būdami kataloge, matysite kelis iš šių aplankų:

         - Dalyje **Taikomosios programos talpykla** eikite į Talpykla ir panaikinkite visus failus talpyklos vietoje: %appdata%\Microsoft\teams\application cache\cache.

        - Dalyje **Blob_storage** panaikinkite visus failus: %appdata%\Microsoft\teams\blob_storage.

        - Dalyje **Cache** panaikinkite visus failus: %appdata%\Microsoft\teams\Cache.

        - Dalyje **databases** panaikinkite visus failus: %appdata%\Microsoft\teams\databases.

        - Dalyje **GPUCache** panaikinkite visus failus: %appdata%\Microsoft\teams\GPUcache.

        - Dalyje **IndexedDB** panaikinkite .db failą: %appdata%\Microsoft\teams\IndexedDB.

        - Dalyje **Local Storage** panaikinkite visus failus: %appdata%\Microsoft\teams\Local Storage.

        - Galiausiai dalyje **tmp** panaikinkite bet kurį failą: %appdata%\Microsoft\teams\tmp.

    4. Iš naujo paleiskite „Teams“ klientą.
