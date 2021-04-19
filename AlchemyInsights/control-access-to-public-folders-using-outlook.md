---
title: Prieigos prie viešųjų aplankų valdymas naudojant "Outlook"
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816748"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Prieigos prie viešųjų aplankų valdymas naudojant "Outlook"

Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook":

1. Naudoti `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"  
$false: neleisti vartotojams pasiekti viešųjų aplankų programoje "Outlook". – tai yra numatytoji reikšmė.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Pastaba: ši procedūra gali valdyti tik ryšius su "Outlook" darbalaukiu, skirta "Windows" klientams. Vartotojai gali toliau pasiekti viešuosius aplankus naudodami OWA arba "Outlook", skirtą "Mac".

Daugiau informacijos žr. ["Outlook" valdomi ryšiai](https://aka.ms/controlpf) su viešais aplankais.
