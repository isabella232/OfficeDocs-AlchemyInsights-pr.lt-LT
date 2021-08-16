---
title: Prieigos prie viešųjų aplankų valdymas naudojant Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032566"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Prieigos prie viešųjų aplankų valdymas naudojant Outlook

Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami Outlook:

1. Naudoti `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: leisti vartotojams pasiekti viešuosius aplankus Outlook  
$false: neleisti vartotojui pasiekti viešųjų aplankų Outlook. – tai yra numatytoji reikšmė.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Pastaba: ši procedūra gali valdyti tik ryšius su "Outlook", skirtais Windows klientams. Vartotojai gali toliau pasiekti viešuosius aplankus naudodami "OWA" arba "Outlook", skirtą "Mac".

Daugiau informacijos žr. [Valdomi ryšiai su viešais aplankais Outlook](https://aka.ms/controlpf) daugiau informacijos.
