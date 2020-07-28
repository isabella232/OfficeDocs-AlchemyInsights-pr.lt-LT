---
title: "\"Office\" taikomųjų programų naujinimo kanalų keitimas"
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
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439392"
---
# <a name="change-update-channels-for-office-apps"></a>"Office" taikomųjų programų naujinimo kanalų keitimas

Norėdami pasirinkti norimą naujinimo kanalą, naudokite naujas "Office" diegimo programas, tada įdiekite (arba įdiekite iš naujo) "Office" programas. Daugiau informacijos rasite [Programinės įrangos atsisiuntimo parametrų valdymas "Office 365".](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) 

**Pastaba** Naujinimo kanalas, pasirinktas naudojant "Office" programinės įrangos atsisiuntimo parametrus, taikomas visiems vartotojams, atliekantiems naujus diegimus naudojant O365 portalą. Daugiau informacijos rasite ["Microsoft 365" arba "Office 2019" atsisiuntimas ir diegimas arba diegimas iš naujo asmeniniame arba "Mac" kompiuteryje](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Esamų "Office" įrenginių, naudokite Office diegimo įrankis (ODT) pereiti į kitą naujinimo kanalą:  

1. Atsisiųskite naujausią "Office" diegimo įrankį (setup.exe) iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Nustatykite kanalo, į kurį norite perjungti, pavadinimą. Daugiau informacijos ieškokite ["Office" diegimo įrankio konfigūravimo parinktys](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Sukurkite konfigūracijos XML failą, kuriame būtų nurodytas atitinkamas kanalo pavadinimas, pvz., update.xml.  
    A. <Configuration>  
    B. <Atnaujinimai **kanalas = "Kas mėnesį"** />  
    C. </Configuration>
4. Didesnių teisių komandinėje eilutėje pereikite į aplanko vietą, kurioje gyvena setup.exe, ir vykdykite šią komandą:  
    A. setup.exe /configure update.xml
5. Paleiskite "Office" programą (pvz., "Excel"), tada pasirinkite **Failo**  >  **abonementas**. Sekcijoje Produkto informacija pasirinkite **Naujinti parinktis**  >  **Naujinti dabar**.

Jei norite gauti daugiau informacijos, [Sužinokite, kaip perjungti naujinimo kanalus esamų Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Perjungti naujinimo kanalus pasirinktos grupės vartotojų arba naudojant konfigūracijos tvarkyklė (SCCM), konfigūruoti naujinimo kanalo parametrą naudojant GPO. Daugiau informacijos rasite ["Microsoft 365" programėlių naujinimo kanalų apžvalga](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Norėdami gauti daugiau informacijos, [sužinokite, kaip valdyti "Office 365 ProPlus" kanalus IT specialistams](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) ir [tvarkyti "Microsoft 365" programėlių naujinimus naudojant "Microsoft Endpoint Configuration Manager".](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)