---
title: 726 blokavimo el. pašto peradresavimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478345"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="74a21-102">Pašto peradresavimo blokavimas arba atblokavimas</span><span class="sxs-lookup"><span data-stu-id="74a21-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="74a21-103">Norėdami įjungti arba išjungti konkrečios pašto dėžutės pašto peradresavimą, skaitykite [pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="74a21-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="74a21-104">Nuomotojo lygmenyje išorinio peradresavimo valdymas atliekamas naudojant siuntimo pašto šiukšlių strategiją.</span><span class="sxs-lookup"><span data-stu-id="74a21-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="74a21-105">Galite patikrinti siuntimo pašto šiukšlių filtravimo strategiją iš saugos ir atitikties centro [čia](https://protection.office.com/antispam) arba naudodami [komandą Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="74a21-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="74a21-106">Jei gaunate šį klaidos pranešimą: **"550 5.7.520" prieiga uždrausta, jūsų organizacija neleidžia naudoti išorinio peradresavimo "**, įsitikinkite, kad strategija sukonfigūruota įgalinti išorinį automatinį persiuntimą.</span><span class="sxs-lookup"><span data-stu-id="74a21-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="74a21-107">**Pastaba:** Rekomenduojama palikti išorinį automatinį persiuntimą jūsų numatytoje siuntimo pašto šiukšlių filtro strategijoje ir įgalinti ją tik vartotojams, kuriems reikia išorinio persiuntimo sukuriant pasirinktinę strategiją tiems vartotojams.</span><span class="sxs-lookup"><span data-stu-id="74a21-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="74a21-108">Galite paskaityti daugiau [konfigūravus išorinį pašto persiuntimą "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)".</span><span class="sxs-lookup"><span data-stu-id="74a21-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>