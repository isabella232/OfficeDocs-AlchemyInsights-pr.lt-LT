---
title: Taikomosios programos tarpinio serverio konfigūracija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885521"
---
# <a name="app-proxy-configuration"></a>Taikomosios programos tarpinio serverio konfigūracija

1. Norėdami sužinoti, kaip konfigūruoti taikomosios programos tarpinio serverio taikomąją programą "Azure AD", kad savo vietines taikomąsias programas būtų galima atskleisti debesyje, Sužinokite, [kaip sukonfigūruoti taikomosios programos tarpinio serverio taikomąją programą](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Bendroji autentifikacija (SSO) leidžia vartotojams pasiekti taikomąją programą neautentifikuojant kelių kartų. Jis leidžia vienam autentifikavimui įvykti debesyje, prieš "Azure Active Directory", ir leidžia tarnybai arba jungčiai apsimokite vartotoju, kad būtų galima atlikti papildomas autentifikavimo problemas iš taikomosios programos. Norėdami sužinoti daugiau, Sužinokite, [kaip konfigūruoti bendrąją autentifikacija taikomosios programos tarpinio serverio taikomajai programai](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Naudokite [šį straipsnį](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) , kad išspręstumėte įprastas problemas, su kuriomis susiduria žmonės kurdami naują taikomosios programos tarpinio serverio taikomąją programą.
4. Jei kyla problemų nustatant back-end autentifikavimą taikomojoje programoje, gali reikėti [Šalinti tarpinio serverio "Kerberos" įgaliojimų perdavimo konfigūracijas](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) arba stebėti [taikomosios programos konfigūravimą su "pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ", kad išspręstumėte problemą.
