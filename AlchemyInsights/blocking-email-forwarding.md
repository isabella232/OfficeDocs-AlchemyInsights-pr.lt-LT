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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219863"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="18c4c-102">Pašto peradresavimo blokavimas arba atblokavimas</span><span class="sxs-lookup"><span data-stu-id="18c4c-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="18c4c-103">Norėdami įjungti arba išjungti konkrečios pašto dėžutės pašto peradresavimą, skaitykite [pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="18c4c-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="18c4c-104">Nuomotojo lygiu išorinio peradresavimo valdymas atliekamas naudojant siuntimo pašto šiukšlių strategiją.</span><span class="sxs-lookup"><span data-stu-id="18c4c-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="18c4c-105">Jei jis nustatytas kaip išjungtas arba automatinis, gali būti blokuojamų laiškų peradresavimas su klaida "550 5.7.520" prieiga uždrausta, jūsų organizacija neleidžia naudoti išorinio peradresavimo ".</span><span class="sxs-lookup"><span data-stu-id="18c4c-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="18c4c-106">Vėliau, jei buvo nustatyta, kad peradresavimas yra užblokuotas, tai yra klaida, kurią matys vartotojai.</span><span class="sxs-lookup"><span data-stu-id="18c4c-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="18c4c-107">Jei peradresavimas užblokuotas, įsitikinkite, kad strategija sukonfigūruota įgalinti išorinius Autoforward.</span><span class="sxs-lookup"><span data-stu-id="18c4c-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="18c4c-108">Galite patikrinti siuntimo pašto šiukšlių filtravimo strategiją iš saugos ir atitikties centro arba paleisdami komandą gauti HostedOutboundSpamFilterPolicy | FL pavadinimas, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="18c4c-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="18c4c-109">Jei norite nustatyti automatinį persiuntimą, ta pati komanda parodys jums strategijos būseną dabar.</span><span class="sxs-lookup"><span data-stu-id="18c4c-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="18c4c-110">Pastaba: rekomenduojama palikti išorinį automatinį persiuntimą jūsų numatytoje siuntimo pašto šiukšlių filtro strategijoje ir įgalinti ją tik vartotojams, kuriems reikia išorinio persiuntimo sukuriant pasirinktinę strategiją tiems vartotojams.</span><span class="sxs-lookup"><span data-stu-id="18c4c-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="18c4c-111">Galite paskaityti daugiau [konfigūravus išorinį pašto persiuntimą "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)".</span><span class="sxs-lookup"><span data-stu-id="18c4c-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>