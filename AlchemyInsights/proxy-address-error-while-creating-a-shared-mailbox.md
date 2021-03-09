---
title: Tarpinio serverio adreso klaida kuriant bendrinamą pašto dėžutę
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568298"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="16b43-102">Tarpinio serverio adreso klaida kuriant pašto dėžutę arba kitą objektą, kuriam įgalintas el. paštas</span><span class="sxs-lookup"><span data-stu-id="16b43-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="16b43-103">Jei bandėte kurti el. pašto funkciją palaikantį objektą (pašto dėžutę, bendrinamą pašto dėžutę ir kt.) ir gavote klaidos pranešimą "tarpinio serverio adresas" SMTP:alias@domain.com "jau naudojamas...", jūsų pasirinktas elektroninio pašto adresas jau yra įtrauktas į kitą jūsų organizacijoje esantį objektą, kuriame įgalintas el. laiškas.</span><span class="sxs-lookup"><span data-stu-id="16b43-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="16b43-104">Jums reikia surasti vartotoją, grupę, bendrinamą pašto dėžutę arba viešąjį aplanką, kuriame yra šis elektroninio pašto adresas ir jį panaikinti arba pakeisti jo elektroninio pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="16b43-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="16b43-105">Tada galite sukurti naują el. pašto objektą su atlaisvintomis el. pašto adresu.</span><span class="sxs-lookup"><span data-stu-id="16b43-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="16b43-106">Naudokite iešką pagrindiniame puslapyje, kad ją rastumėte.</span><span class="sxs-lookup"><span data-stu-id="16b43-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="16b43-107">Taip pat galite naudoti šią "Exchange Online PowerShell" komandą, kad galėtumėte ją rasti:</span><span class="sxs-lookup"><span data-stu-id="16b43-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="16b43-108">Jei nenorite panaikinti esamo elektroninio pašto adreso, pasirinkite naują naujo objekto, kurį kuriate, elektroninio pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="16b43-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  