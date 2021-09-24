---
title: Antrinio domeno įtraukimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506483"
---
# <a name="adding-a-sub-domain"></a>Antrinio domeno įtraukimas

Antrinius domenus galima įtraukti į tą patį arba kitą nuomotoją nei pirminis domenas. Bet kuriuo atveju turite valdyti savo DNS parametrus savo registratoriaus svetainėje. Jei leidžiate "Microsoft" valdyti SAVO DNS parametrus naudojant NS įrašus arba jei įsigijote domeną iš "Microsoft", pirmiausia negalite įtraukti padomenių.

Pirmiausia įtraukite pirminį domeną, tada įtraukite poaplankių domeną. Jei padomenio nuomotojas yra tame pačiame nuomotoje, papildomo patvirtinimo nereikia. Jei subdomeno įtraukimas į atskirą nuomotoją, dns txt įrašas būtinas nuosavybės tikrinimui prieš įtraukiant domeną ir papildomus pasirinktų tarnybų DNS įrašus.

- Norėdami įtraukti domeną arba padomenio, vykdykite vediklį Įtraukti domeną [arba](https://admin.microsoft.com/Adminportal#/Domains/Wizard)rankiniu būdu įtraukite domeną arba padomenio, nueikite į   >  **Domenų įtraukimas**  >  **domeno nustatymas**.

Jei reikia:

- Norėdami pakeisti, kas valdo esamo domeno DNS parametrus, eikite **į Parametrai** Domenai , pažymėkite žymės langelį šalia  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **domeno,** tada pasirinkite Valdyti DNS . Vedlyje pasirinkite Įtraukti **savo DNS įrašus ir užbaikite** vediklį.
- Norėdami įtraukti antrinių domenų į "Microsoft" įsigytą domeną, pirmiausia perkelkite domeną į kitą registratorių, tada atlikite anksčiau nurodytus pokyčius, kad tvarkydami savo DNS įrašus. Instrukcijų ieškokite [Domeno perkėlimas iš "Microsoft" į kitą pagrindinį kompiuterį](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Jei gaunate klaidos pranešimą, kad jūsų domeną jau naudoja kiti organizacijos nariai arba žmonės, pirmiausia turėsite perimti šią nevaldomąjį abonementą prieš naudodami domeną. Instrukcijas [žr. Nevaldomąjį katalogą perimti administratoriaus](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)teisėmis "Azure Active Directory".
