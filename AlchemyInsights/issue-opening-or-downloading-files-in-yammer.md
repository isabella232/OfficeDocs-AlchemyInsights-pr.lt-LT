---
title: Failų atidarymo arba atsisiuntimo "Yammer" problema
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148334"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Failų atidarymo arba atsisiuntimo "Yammer" problema

Klasikinis "Yammer" palaiko kelias failų nusiuntimo į pranešimus ir grupes parinktį. Atsižvelgiant į tinklo konfigūraciją, failai, kurie yra numatytieji kaip "SharePoint" saugomi.

Failų parinkiklis naujajame "Yammer" dar nepalaiko visų klasikiniame "Yammer" parinkčių. Ateityje atnaujinus bus pridėtos papildomos funkcijos. Daugiau informacijos rasite [Failo arba vaizdo pridėjimas prie "Yammer" pokalbio skelbimo](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nepavyksta atidaryti arba atsisiųsti failo**  

Failas gali būti nusiųstas į "Yammer", bet taip pat gali būti susietas su "SharePoint Online" failu. Norėdami pašalinti triktis, pirmiausia turite nustatyti failo vietą. Jei failas buvo įkeltas į "Yammer", jis turės *.yammer.com URL. Įsitikinkite, kad būtini URL ir IP adresai yra atblokuoti. Daugiau informacijos rasite tinklaraščio įraše ["Yammer" užkoduoto IP adresų naudojimas nerekomenduojamas](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Patikrinkite, ar vartotojas, kuris taip pat yra visuotinis administratorius, gali atsisiųsti failą. Jei failas yra privatus, gali tekti naudoti asmeninio turinio režimą. Daugiau informacijos rasite ["Yammer" asmeninio turinio stebėjimas](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**"Yammer" tinklo lygio svečiai ir failai "SharePoint Online"**  

["Yammer" tinklo lygio svečiai](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nenaudoja "Azure AD B2B" ir yra vidiniai "Yammer" tarnybai, todėl jie negali pasiekti "Yammer" failų, saugomų "SharePoint". Sukurkite išorinį AAD B2B vartotoją, kuris gali pasiekti dokumentų bibliotekas "SharePoint Online" naudodamas tą tapatybę. Informacijos apie būsimą "Azure AD B2B" svečio palaikymą "Yammer", ieškokite ["Business-to business" (B2B) svečio palaikymas "Yammer Preview" – klientų sąlygos ir DUK.](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)