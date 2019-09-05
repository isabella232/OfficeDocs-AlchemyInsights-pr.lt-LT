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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="81215-102">Pašto dėžučių audito įjungimas</span><span class="sxs-lookup"><span data-stu-id="81215-102">Enable mailbox auditing</span></span>

<span data-ttu-id="81215-103">Norėdami įgalinti vieno vartotojo arba visos organizacijos pašto dėžučių tikrinimą, iš nuotolinio maitinimo apvalkalo reikia paleisti toliau nurodytas cmdlet.</span><span class="sxs-lookup"><span data-stu-id="81215-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="81215-104">**Vienas vartotojas**</span><span class="sxs-lookup"><span data-stu-id="81215-104">**Single User**</span></span>
  
<span data-ttu-id="81215-105">Set-Mailbox-tapatybė "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="81215-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="81215-106">**Organizacijos**</span><span class="sxs-lookup"><span data-stu-id="81215-106">**Organization**</span></span>
  
<span data-ttu-id="81215-107">Gauti-Mailbox-ResultSize neribotas-filtras {RecipientTypeDetails-EQ "vartotojo pašto dėžutė"} | Set-Mailbox – AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="81215-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="81215-108">sužinoti daugiau, sužinok daugiau</span><span class="sxs-lookup"><span data-stu-id="81215-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

