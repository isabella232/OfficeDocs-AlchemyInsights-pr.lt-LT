---
title: Nepavyksta siųsti/gauti el. laiško į/iš "Office 365", nes TLS 1,0 ir TLS 1,1 neįgalūs
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747123"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="e87e5-102">Nepavyksta siųsti/gauti el. laiško į/iš "Office 365", nes TLS 1,0 ir TLS 1,1 neįgalūs</span><span class="sxs-lookup"><span data-stu-id="e87e5-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="e87e5-103">Kaip patvirtino pranešimų centro pašto MC229914, TLS 1,0 ir TLS 1,1 nuteistųjų pradėjo vykdyti "Exchange Online" pašto srauto pabaigos taškus.</span><span class="sxs-lookup"><span data-stu-id="e87e5-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="e87e5-104">Netrukus "Office 365" nebepriims TLS 1,0 ir TLS 1,1 elektroninio pašto ryšių iš išorinių šaltinių.</span><span class="sxs-lookup"><span data-stu-id="e87e5-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="e87e5-105">Be to, "Exchange Online" niekada nenaudos TLS 1,0 arba 1,1 siųsti siunčiamus laiškus.</span><span class="sxs-lookup"><span data-stu-id="e87e5-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="e87e5-106">Jei susiduriate su problemomis dėl TLS 1,0 arba 1,1 negalios, galite susidurti su viena iš šių klaidų –</span><span class="sxs-lookup"><span data-stu-id="e87e5-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="e87e5-107">Siuntėjas gauna NDR Bounce atgal – "421 4.4.2" sujungimas dėl "SocketError"</span><span class="sxs-lookup"><span data-stu-id="e87e5-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="e87e5-108">Klaida, esanti vietinio serverio, kuris siunčia laišką į pareigūno 365 – "421 4.4.2" jungtį, dėl "SocketError", eilėje.</span><span class="sxs-lookup"><span data-stu-id="e87e5-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="e87e5-109">Klaida siunčiant jungties [protokolo prisijungimo](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveryje laišką siunčiant į "Office 365" – TLS derybos nepavyko dėl klaidos SocketError</span><span class="sxs-lookup"><span data-stu-id="e87e5-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="e87e5-110">Klaida siuntimo arba gavimo jungties protokolo logaritme – "451" 5.7.3 turi būti pirmoji "STARTTLS" komanda.</span><span class="sxs-lookup"><span data-stu-id="e87e5-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="e87e5-111">Jei susiduriate su bet kuria iš aukščiau nurodytų klaidų, įsitikinkite, kad serveryje, kuris siunčia arba gauna laišką, TLS 1,2 įjungėte patikrindami šiuos registro raktus –</span><span class="sxs-lookup"><span data-stu-id="e87e5-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="e87e5-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klientas] **"DisabledByDefault" = DWORD: 00000000 "= DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ serveris] **" DisabledByDefault "= DWORD: 00000000" įjungtas "= DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="e87e5-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="e87e5-113">Jei pakeisite anksčiau nurodytus registro raktus, Norėdami įgalinti TLS 1,2, iš naujo paleiskite serverį, kad įsigaliotų pakeitimai.</span><span class="sxs-lookup"><span data-stu-id="e87e5-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="e87e5-114">Taip pat įsitikinkite, kad įdiegėte naujausius "Windows" ir "Exchange" naujinimus.</span><span class="sxs-lookup"><span data-stu-id="e87e5-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="e87e5-115">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="e87e5-115">For more information, see:</span></span>

- [<span data-ttu-id="e87e5-116">"Exchange Server" TLS nuorodos, 1 dalyje: Pasiruošimas TLS 1,2-"Microsoft" technologijų bendruomenė</span><span class="sxs-lookup"><span data-stu-id="e87e5-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="e87e5-117">"Exchange Server" TLS rekomendacijų 2 dalyje: TLS 1,2 ir klientų tapatybės nustatymas nenaudojant IT – "Microsoft" technologijų bendruomenė</span><span class="sxs-lookup"><span data-stu-id="e87e5-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="e87e5-118">El. pašto scenarijų supratimas, jei negalima susitarti dėl TLS versijų naudojant "Exchange Online" – "Microsoft" technologijų bendruomenė</span><span class="sxs-lookup"><span data-stu-id="e87e5-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
