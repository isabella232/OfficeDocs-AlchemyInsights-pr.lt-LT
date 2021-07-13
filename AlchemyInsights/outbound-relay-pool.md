---
title: Siuntimo perdavimo telkinys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381719"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="cd672-102">Siuntimo perdavimo telkinys</span><span class="sxs-lookup"><span data-stu-id="cd672-102">Outbound relay pool</span></span>

<span data-ttu-id="cd672-103">"Microsoft" keičia el. laiškų perdavimo arba persiuntimo per Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cd672-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="cd672-104">Tam tikrų scenarijų pranešimai persiunčiami arba perduodami per Microsoft 365 naudojant specialų perdavimo telkinį.</span><span class="sxs-lookup"><span data-stu-id="cd672-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="cd672-105">Laiškai, siunčiami naudojant perdavimo telkinį, gali būti gavėjo nepageidaujamų laiškų aplanke.</span><span class="sxs-lookup"><span data-stu-id="cd672-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="cd672-106">Daugiau informacijos žr. [Siuntimo pristatymo telkiniai](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="cd672-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="cd672-107">Norėdami išvengti scenarijaus naudodami perdavimo telkinį, įsitikinkite, kad persiųsti / perduoti laiškai atitinka vieną iš šių kriterijų:</span><span class="sxs-lookup"><span data-stu-id="cd672-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="cd672-108">Siunčiamas siuntėjas yra priimtas nuomotojo domenas.</span><span class="sxs-lookup"><span data-stu-id="cd672-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="cd672-109">Siuntėjo strategijos sistema (SPF) pereina, kai pranešimas Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cd672-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="cd672-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cd672-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="cd672-111">Pranešimai, kurie atitinka anksčiau nurodytus kriterijus, nėra perteikite per perdavimo telkinį.</span><span class="sxs-lookup"><span data-stu-id="cd672-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="cd672-112">Jei jūsų domeno MX įrašas yra nukreiptas į trečiosios šalies arba vietinį serverį, naudokite patobulintą filtravimą, kad įsitikintumėte, jog SPF tikrinimas yra tinkamas gaunamiesiems el. laiškams ir kad el. laiškai nebūtų siunčiami per perdavimo telkinį.</span><span class="sxs-lookup"><span data-stu-id="cd672-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="cd672-113">**Kaip sužinoti, ar mus paveikė relės telkinys?**</span><span class="sxs-lookup"><span data-stu-id="cd672-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="cd672-114">Jei jūsų persiunčiami arba persiunčiami el. laiškai naudoja vieną iš aukščiau nurodytų kriterijų, pranešimai nebus perduodami per perdavimo telkinį.</span><span class="sxs-lookup"><span data-stu-id="cd672-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="cd672-115">Tačiau, jei pranešimas siunčiamas per perdavimo telkinį, siuntimo serverio IP yra diapazone 40.95.0.0/16, o siuntimo serverio vardas pavadinime yra **rly.**</span><span class="sxs-lookup"><span data-stu-id="cd672-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

