---
title: Keli objektai turi tą patį el. pašto adresą kaip ir tapatybė
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439190"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Keli objektai turi tą patį el. pašto adresą kaip ir tapatybė

**Keli objektai**

Viena iš dažniausiai pasitaikančių šios klaidos priežasčių yra neįmanoma tinkamai nukreipti "Outlook Web Access" užklausos, jei yra keli objektai, turintys tą patį el. pašto adresą kaip tapatybė. Norėdami rasti šiuos objektus, vykdykite šias komandas:

· Gavėjas<email address>

· Gaukite vartotoją<email address>

· Get-User <email address> -SoftDeletedUser Get-User -SoftDeletedUser Get-User -SoftDeletedUser

· Susisiekite su mumis<email address>

· Get-Mailbox -PublicFolder Gauti pašto dėžutės <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox Gauti pašto dėžutės - IncludeSoftDeletedMailbox

· Get-Mailbox -InactiveMailboxOnly Gauti pašto dėžutės- <email address> InactiveMailboxOnly

Norėdami išspręsti šią problemą, pašalinkite kelis objektus su tuo pačiu el. pašto tapatybe ir įsitikinkite, kad yra vienas objektas su konkrečiu el. pašto tapatybe ir kad jo gavėjo tipas yra UserMailbox.

**Tas pats adresas naudojamas įmonėms ir vartotojų pašto dėžutėms**

Kita priežastis yra, kai tas pats adresas naudojamas verslo ir vartotojų pašto dėžutės. Tokiu atveju vartotojas turi pakeisti savo pagrindinį vartotojo pseudonimą, kol kavinė palaiko šį scenarijų. Tai nuolatinė klaida, kuri neišeina be įsikišimo.

Išsamesnės informacijos [ieškokite "Microsoft" paskyros el. pašto adreso arba telefono numerio keitimas.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)