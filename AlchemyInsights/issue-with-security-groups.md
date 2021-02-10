---
title: Problema su saugos grupėmis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177499"
---
# <a name="issue-with-security-groups"></a>Problema su saugos grupėmis

**Jei gaunate tinklo klaidos AADDS104**

Netinkamos tinklo saugos grupės taisyklės yra Dažniausios "Azure Active Directory" domenų tarnybos (AD DS) tinklo klaidų priežastys. Virtualaus tinklo tinklo saugos grupė turi suteikti prieigą prie konkrečių prievadų ir protokolų. Jei šie prievadai užblokuoti, "Azure" platformoje negalima stebėti arba atnaujinti valdomo domeno. Taip pat paveikė "Azure AD" ir "Azure AD DS" sinchronizavimas. Įsitikinkite, kad paliksite numatytuosius prievadus, kad išvengtumėte paslaugos nutraukimo.

Norėdami suprasti ir išspręsti bendruosius įspėjimus apie tinklo saugos grupės konfigūravimo problemas, skaitykite [saugos grupių įtraukimas ir tikrinimas](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
