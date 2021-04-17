---
title: „Yammer“ pranešimai
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833587"
---
# <a name="notifications-in-yammer"></a>„Yammer“ pranešimai

Kad įspėtų jus apie naują veiklą atitinkamuose pokalbiuose, [„Yammer“ siunčia pranešimus](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) el. paštu arba, jei naudojate „Yammer“ mobiliajame įrenginyje, – „Push“ pranešimus. Pagal numatytuosius nustatymus „Yammer“ siunčia pranešimus apie daugelio tipų veiklą jūsų tinkle. Vartotojai gali atnaujinti savo el. pašto parametrus „Yammer“ svetainėje, o „Push“ pranešimus galima sukonfigūruoti mobiliųjų įrenginių programėlėje. 

„Yammer“ palaiko [interaktyvius el. laiškus programoje „Outlook“](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Kai kurie el. laiškai (laiškų kopijos) taps interaktyvūs internetinėje „Outlook“. Būsimame naujinime tai bus pristatyta kitose „Outlook“ versijose.

**„Yammer“ pranešimų tipai**

- El. laiškai (atnaujinimai grupėje, kažkas pakviečia jus į grupę, gaunate pranešimą į savo aplanką Gauta ir pan.)
- „Push“ pranešimai (siunčiami į mobiliuosius įrenginius, kai jus pamini, kai gaunate pranešimą į savo aplanką Gauta ir pan.)
- Darbalaukyje iššokantys langai (jei turite įdiegę „Yammer“ kompiuterio taikomąją programą, vartotojams bus rodomi pranešimai, vadinami laikinaisiais pranešimais.)
- Pranešimai su varpelio piktograma („Yammer“ svetainėje vartotojai matys pranešimus apie įvairius įvykius. Šie pranešimai ne visada turės susietą el. paštu siunčiamą arba „push“ pranešimą.)

Galite gauti daugiau [išsamios informacijos apie pranešimus](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Pranešimų valdymas**

Savo pranešimus turi valdyti patys vartotojai. Informacijos galite rasti [Kaip įjungti ir išjungti „Yammer“ el. pašto ir mobiliuosius pranešimus](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratoriai negali išjungti visų pranešimų ar jų valdyti vartotojų vardu. Administratoriai gali [valdyti logotipą, įtraukiamą į el. laiškus, ir nurodyti, ar vartotojai turi patvirtinti pranešimus,](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) siunčiamus el. paštu.

**Pranešimai el. paštu, siunčiami daugeliui jūsų organizacijos vartotojų**

Kartais „Yammer“ siųs vieną pranešimą el. paštu, kurį gaus daug daugiau jūsų organizacijos vartotojų, nei tikėtasi. Taip nutinka, kai į „Yammer“ įtraukiamas platinimo sąrašas arba kito tipo ne individualus el. pašto adresas. „Yammer“ ne visada žino, ar el. pašto adresas priklauso vienam vartotojui, ar tai yra el. pašto adresas, kuriuo vienas el. laiškas bus pristatytas daugeliui gavėjų. Kai iškyla ši problema, turite imtis veiksmų, kad „Yammer“ [sustabdytumėte (išjungtumėte) netinkamą vartotoją su tuo el. pašto adresu](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). 

Norėdami sumažinti šios problemos tikimybę, turėtumėte:

1. [Įgalinti „Office 365“ tapatybę](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) „Yammer“ vartotojams.
2. Užblokuoti išorinius siuntėjus, kad jie negalėtų siųsti el. laiškų jūsų organizacijai, arba apriboti siuntėjus iki priklausančiųjų patvirtintų siuntėjų sąrašui.

Jei iškyla ši problema:

1. Identifikuokite el. laiško gavėją, kuris turėtų atitikti „Yammer“ užregistruotą vartotoją. Pvz., pardavimo-skyrius@fabrikam.com yra siuntimo sąrašas, skirtas visiems žmonėms iš pardavimo skyriaus. Šis siuntimo sąrašas turėtų būti identifikuojamas iš vartotojų gauto „Yammer“ el. laiško.
2. Naudokite [tinklo administravimo funkciją Išjungti (sustabdyti)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users), kad sustabdytumėte vartotoją, turintį el. pašto adresą pardavimo-skyrius@fabrikam.com. Sustabdymas gali būti anuliuojamas, todėl tai saugesnė parinktis nei panaikinimas. Vartotojas panaikinamas automatiškai po 90 dienų.
3. Taip pat galite peržiūrėti [Vartotojų eksportavimas](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), kad identifikuotumėte kitus ne vartotojų el. pašto adresus, kurie turėtų būti sustabdyti.
