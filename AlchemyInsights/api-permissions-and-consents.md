---
title: API teisės ir sutikimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932105"
---
# <a name="api-permissions-and-consent"></a>API teisės ir sutikimas

Su ""Microsoft" tapatybės platforma" integruojamos taikomosios programos atitinka autorizavimo modelį, kuris suteikia vartotojams ir administratoriams galimybę kontroliuoti, kaip galima pasiekti duomenis. Autorizavimo modelio diegimas buvo atnaujintas "Microsoft" tapatybės platforma pabaigos taške. Ji pakeičia, kaip programa turi sąveikauti su "Microsoft" tapatybės platforma. [Teisės ir sutikimas "Microsoft" tapatybės platforma galinio](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) punkto apima pagrindines šio autorizavimo modelio sąvokas, įskaitant aprėptis, teises ir sutikimą.

""Azure Active Directory" [("Azure AD")](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) sutikimo sistema leidžia lengvai kurti kelių nuomotojų žiniatinklio ir vietinių klientų taikomąsias programas. Šios taikomosios programos leidžia prisijungti pagal vartotojų paskyras iš "Azure AD" nuomotojo, kuris skiriasi nuo to, kuriame registruota taikomoji programa. Jiems taip pat gali reikėti pasiekti žiniatinklio API, pvz., "Microsoft "Graph"" API (norint pasiekti "Azure AD", "Intune" ir paslaugas "Microsoft 365") ir kitus ""Microsoft" paslaugos" API, be jūsų žiniatinklio API.

