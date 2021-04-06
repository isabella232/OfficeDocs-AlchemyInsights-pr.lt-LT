---
title: Panaikintų "Microsoft 365" grupės atkūrimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597451"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="8b203-102">Panaikintų "Microsoft 365" grupės atkūrimas</span><span class="sxs-lookup"><span data-stu-id="8b203-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="8b203-103">Panaikintų "Microsoft 365" grupių arba "Microsoft Teams" galite atkurti per 30 dienų nuo panaikinimo.</span><span class="sxs-lookup"><span data-stu-id="8b203-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="8b203-104">Eikite į ["Microsoft 365" administravimo centrą,](https://aka.ms/RestoreDeletedGroup) kad prisiregistruotų, ir išvardikite panaikintas grupes ir komandas.</span><span class="sxs-lookup"><span data-stu-id="8b203-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="8b203-105">**Pastaba:** Prisijunkite naudodami paskyrą, priskirtą nuomotojo administratoriui arba grupių administratoriaus vaidmeniui.</span><span class="sxs-lookup"><span data-stu-id="8b203-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="8b203-106">Pasirinkite panaikinti "Microsoft 365" grupę / "Teams", kuri bus atkurta, ir **spustelėkite atkurti grupę**.</span><span class="sxs-lookup"><span data-stu-id="8b203-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="8b203-107">Jei grupės atkurti negalima dėl nesuderinamo SMTP adreso, naudokite šią komandą, kad rastumėte konfliktą keliantį objektą ir pašalintumėte SMTP adresą:</span><span class="sxs-lookup"><span data-stu-id="8b203-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="8b203-108">**Pastaba:** Kai kuriais atvejais gali užtrukti iki 24 valandų, kol grupė ir visi jos duomenys bus atkurti.</span><span class="sxs-lookup"><span data-stu-id="8b203-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="8b203-109">Daugiau informacijos arba sužinokite, kaip atkurti grupes naudojant "PowerShell", žr. [Panaikintų "Microsoft 365" grupės atkūrimas.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="8b203-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>