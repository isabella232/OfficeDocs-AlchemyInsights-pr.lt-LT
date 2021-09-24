---
title: "\"Microsoft\" vardų serverių keitimas į savo DNS įrašų valdymą"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506608"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>"Microsoft" vardų serverių keitimas į savo DNS įrašų valdymą

Anksčiau pakeitėte savo NS įrašus į "Microsoft" (ns1.bdm.microsoftonline.com), bet nusprendėte dabar valdyti savo DNS įrašus:

Savo domenų registratoriaus svetainėje pakeiskite vardų serverį atgal į registratorių arba ankstesnį parametrą. Jei esate susipažinę su DNS, kreipkitės į domeno registratoriaus palaikymo tarnybą. Atkreipkite dėmesį, kad vardų serverio pakeitimai gali užtrukti iki 48 valandų, kad būtų galima išplatinti. 

1. Administravimo Microsoft 365 eikite į **Parametrai** domenai , pažymėkite žymės langelį šalia  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **domeno** ir pasirinkite Valdyti DNS . 

2. Vedlyje pasirinkite Įtraukti **savo DNS įrašus ir užbaikite** vediklį. Tai pakeičia, kaip valdomas JŪSŲ DNS, tada leidžia įtraukti pasirinktinius DNS įrašus, reikalingus jūsų pasirinktoms tarnyboms palaikyti.

Taip pat, jei pakeitėte vardų serverio įrašus į "Microsoft" ir turite svetainę, galite įtraukti svetainės DNS įrašus, o ne vėl pakeisti vardų serverius. Daugiau informacijos žr. [DNS įrašų naujinimas, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


