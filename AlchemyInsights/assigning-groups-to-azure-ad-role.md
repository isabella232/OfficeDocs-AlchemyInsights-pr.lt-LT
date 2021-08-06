---
title: Grupių priskyrimas "Azure AD" vaidmeniui
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036248"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Grupių priskyrimas "Azure AD" vaidmeniui

Norėdami priskirti "Azure AD" grupę su "Azure AD" institucijos šaltiniu "Azure AD" vaidmeniui, atlikite šiuos veiksmus:

1. Naujos grupės kūrimas – norėdami sukurti naują grupę:

    a. Prisijunkite prie "Azure AD" administravimo centro naudodami **privilegijuotas vaidmenų administratoriaus arba** **visuotinio administratoriaus** teises.
    b. Pasirinkite **"Azure Active Directory" > Grupės > Visos grupės > Nauja grupė**.
    c. Sukurkite grupę.

2. Priskirkite vaidmenį grupei grupės kūrimo metu arba sukūrus grupę.

    a. Norėdami grupės kūrimo metu grupei priskirti vaidmenį, įjunkite jungiklį **"Azure AD" vaidmenys** gali būti priskirti grupei ir sukurti grupę.
    b. Norėdami priskirti vaidmenį grupei po to, kai jis buvo **sukurtas,** eikite į naujai sukurtos grupės skirtuką Priskirti vaidmenys ir priskirkite vaidmenį grupei.  

**Grupės, priskirtos "Azure AD" vaidmeniui, narystės valdymas**

Norėdami išvengti didesnių teisių, pagal numatytuosius nustatymus tik privilegijuoti vaidmenų administratoriai ir visuotiniai administratoriai gali modifikuoti grupei, kuri priskirta vaidmeniui, narystę. Tačiau jie gali pasirinkti priskirti tokios grupės savininką ir perduoti šią užduotį.

Daugiau informacijos apie debesies grupių priskyrimą "Azure AD" vaidmenims žr. [AD vaidmenų priskyrimas debesies grupei](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Daugiau informacijos apie debesies grupėms priskirtų vaidmenų trikčių diagnostiką žr. [Debesies grupėms priskirtų vaidmenų trikčių diagnostika](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





