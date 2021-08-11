---
title: Programos tarpinio serverio konfigūravimas
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
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951573"
---
# <a name="app-proxy-configuration"></a>Programos tarpinio serverio konfigūravimas

1. Norėdami suprasti, kaip konfigūruoti taikomosios programos tarpinio serverio taikomąją programą "Azure AD", kad jūsų vietinės taikomosios programos būtų matomos debesyje, žr. Kaip konfigūruoti taikomosios [programos tarpinio serverio taikomąją programą](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Bendroji autentifikavimo funkcija (SSO) leidžia vartotojams pasiekti taikomąją programą neautentifikuojant kelis kartus. Tai leidžia atlikti vieną autentifikavimą debesyje, naudojant ""Azure Active Directory"", ir leidžia tarnybai arba jungčiai apsimesti vartotojui atlikti papildomus autentifikavimo iššūkius iš taikomosios programos. Norėdami sužinoti daugiau, [žr. Kaip konfigūruoti bendrąją a prisijungimą prie taikomosios programos tarpinio serverio taikomosios programos](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Naudokite [šį straipsnį norėdami](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) šalinti dažnai pasitaikančių problemų, su kuria susiduria žmonės kurdami naują taikomosios programos tarpinio serverio taikomąją programą, triktis.
4. Jei kyla problemų nustatant programos atsarginį autentifikavimą, gali tekti šalinti ["Kerberos"](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) apriboto perdavimo konfigūracijų triktis taikomosios programos tarpiniame serveris arba vadovautis nurodymais, kaip konfigūruoti taikomąją programą su ["PingAccess",](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) kad išspręsite problemą.
