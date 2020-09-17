---
title: 1065 nuteistųjų iš "IOP" siuntimo IP adreso rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806803"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c6fb4-102">"IOP" siunčiamų IP adreso diapazonų nuteistųjų uždraudimas</span><span class="sxs-lookup"><span data-stu-id="c6fb4-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c6fb4-103">Aptikome galimą organizacijos problemą, kuri (jei nepataisoma spalio 26 d., 2018) gali pažeisti pašto srautą į vietinę arba išorinę paskirties vietą.</span><span class="sxs-lookup"><span data-stu-id="c6fb4-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="c6fb4-104">Kaip buvo pranešta anksčiau, Norėdami supaprastinti IP adresų diapazono valdymą, mes konsoliduojame "Exchange Online Protection" ("e") IP adresų diapazonus, kurie naudojami siųsti ir gauti el. laiškus už "Microsoft 365".</span><span class="sxs-lookup"><span data-stu-id="c6fb4-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="c6fb4-105">Mūsų analizė rodo, kad vienas ar daugiau išorinių elektroninio pašto šaltinių arba paskirties vietų, kurias sukonfigūravote pašto srauto jungtuse, nepriima ryšių iš [čia](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)rodomų IP adresų diapazonų.</span><span class="sxs-lookup"><span data-stu-id="c6fb4-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c6fb4-106">Veikti iki spalio 26 d., siekiant užtikrinti, kad šie šaltiniai ir miestai sutiktų ryšius su visais [paskelbtais EOP IP adresais](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ir iš jų.</span><span class="sxs-lookup"><span data-stu-id="c6fb4-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c6fb4-107">Daugiau informacijos apie šį keitimą ieškokite pranešimų centro pranešimų [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="c6fb4-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c6fb4-108">**Pastaba**: jei anksčiau naudojote IP arba URL skelbimą naudodami HTML, XML ir RSS galinio punkto naujinimus, taip pat turite perkelti į naujas žiniatinklio tarnybas, kad automatizuodami šio tipo naujinimus.</span><span class="sxs-lookup"><span data-stu-id="c6fb4-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="c6fb4-109">Daugiau informacijos ieškokite ["microsoft 365" galinio punkto kategorijų ir "microsoft 365" IP adreso ir URL žiniatinklio tarnybos](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="c6fb4-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
