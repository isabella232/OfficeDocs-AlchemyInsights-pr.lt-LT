---
title: Pašto dėžučių audito įjungimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736261"
---
# <a name="enable-mailbox-auditing"></a>Pašto dėžučių audito įjungimas

Norėdami įgalinti vieno vartotojo arba visos organizacijos pašto dėžučių tikrinimą, iš nuotolinio maitinimo apvalkalo reikia paleisti toliau nurodytas cmdlet.
  
 **Vienas vartotojas**
  
Set-Mailbox-tapatybė "Jane Dow"-AuditEnabled $true
  
 **Organizacijos**
  
Gauti-Mailbox-ResultSize neribotas-filtras {RecipientTypeDetails-EQ "vartotojo pašto dėžutė"} | Set-Mailbox – AuditEnabled $true
  
[sužinoti daugiau, sužinok daugiau](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

