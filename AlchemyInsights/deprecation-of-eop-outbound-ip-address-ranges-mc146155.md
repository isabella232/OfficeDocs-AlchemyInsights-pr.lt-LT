---
title: 1065 EOP siunčiamo IP adreso diapazonųMC146155 nuvertėjimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704605"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="08bf1-102">EOP siunčiamų IP adresų diapazonų nuvertėjimas</span><span class="sxs-lookup"><span data-stu-id="08bf1-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="08bf1-103">Aptikome galimą jūsų organizacijos problemą, kuri (jei nebus ištaisyta iki 2018 m. spalio 26 d.) gali nutraukti pašto srautą į vietines arba išorines paskirties vietas.</span><span class="sxs-lookup"><span data-stu-id="08bf1-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="08bf1-104">Kaip anksčiau pranešta, siekiant supaprastinti IP adresų diapazono valdymą, konsoliduojame "Exchange Online Protection" (EOP) IP adresų diapazonus, naudojamus el. laiškams siųsti ir gauti už "Microsoft 365" ribų.</span><span class="sxs-lookup"><span data-stu-id="08bf1-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="08bf1-105">Mūsų analizė rodo, kad vienas ar daugiau išorinių el. pašto šaltinių ar paskirties vietų, kurias sukonfigūravote pašto srauto jungtyse, nepriima ryšių iš [ČIA](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)rodomų IP adresų diapazonų .</span><span class="sxs-lookup"><span data-stu-id="08bf1-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="08bf1-106">Veikti iki spalio 26 d., siekiant užtikrinti, kad šie šaltiniai ir paskirties vietos priims ryšius su visais [paskelbtais EOP IP adresais](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)ir iš jų .</span><span class="sxs-lookup"><span data-stu-id="08bf1-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="08bf1-107">Jei norite gauti daugiau informacijos apie šį pakeitimą, peržiūrėkite pranešimų centro pranešimų [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="08bf1-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="08bf1-108">**Pastaba**: jei anksčiau naudojote IP arba URL publikavimą per HTML, XML ir RSS galinio punkto naujinimams, taip pat turėtumėte pereiti prie naujų žiniatinklio tarnybų, kad automatizuotumėte šių tipų naujinimus.</span><span class="sxs-lookup"><span data-stu-id="08bf1-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="08bf1-109">Daugiau informacijos ieškokite ["Microsoft 365" galinių punktų kategorijos ir "Microsoft 365" IP adresas ir URL žiniatinklio tarnyba](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="08bf1-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
