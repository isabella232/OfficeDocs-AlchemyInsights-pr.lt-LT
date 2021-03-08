---
title: Bendrųjų problemų sprendimas naudojant DKIM įrašo formatavimą
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525652"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="eee9c-102">Bendrųjų problemų sprendimas naudojant DKIM įrašo formatavimą</span><span class="sxs-lookup"><span data-stu-id="eee9c-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="eee9c-103">Daugelis DKIM nustatymo problemų yra susijusios su klaidingais DNS įrašais.</span><span class="sxs-lookup"><span data-stu-id="eee9c-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="eee9c-104">Norėdami sutvarkyti DKIM nustatymo problemas, patikrinkite, ar teisingai suformatuotas DKIM CNAME įrašas (**ne** txt įrašas).</span><span class="sxs-lookup"><span data-stu-id="eee9c-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="eee9c-105">Daugiau informacijos ieškokite [ką reikia daryti norint rankiniu būdu nustatyti DKIM "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)".</span><span class="sxs-lookup"><span data-stu-id="eee9c-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="eee9c-106">Jei reikia pagalbos dėl DNS įrašų, ieškokite [DNS įrašų kūrimas bet kuriame DNS išteklių nuomos teikėjo, skirto "Office 365"](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="eee9c-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="eee9c-107">Kai savo domeno DNS išteklių nuomos tarnyboje sukuriate arba naujinate savo DKIM DNS įrašus, turėsite palaukti, kol DNS įrašus išplatins.</span><span class="sxs-lookup"><span data-stu-id="eee9c-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
