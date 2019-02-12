---
title: 1065 EOP nuteistųjų siuntimo IP adresas rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934892"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="57289-102">Nuteistųjų, EOP siuntimo IP adresų diapazonai</span><span class="sxs-lookup"><span data-stu-id="57289-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="57289-p101">Aptikome galima problema su jūsų organizacija, kuri (jei negali ištaisyti iki 2018 m. spalio 26 d.) gali sugadinti pašto srautas į jūsų vietinėje ar išorės šalis ir miestus. Kaip anksčiau bendravo, supaprastinti IP adresų diapazoną valdymo, mes konsoliduojate Exchange Online Protection "(EOP) IP adresų diapazonus, kurie yra naudojami siųsti ir gauti el. laiškus ne iš" Office 365 ". Mūsų analizė rodo, kad vienas ar daugiau iš išorės paštu šaltinių ar paskirties vietą, sukonfigūravę pašto srauto jungtys nėra priimti ryšių iš to IP adreso diapazonų parodyta [čia](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="57289-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="57289-106">Veikia iki spalio 26 užtikrinti šių šaltinių ir miestai bus priimti ryšius į ir iš visų [paskelbtas EOP IP adresus](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="57289-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="57289-107">Daugiau informacijos apie šį keitimą, žiūrėkite pranešimų centras registruoja [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)arba [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="57289-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="57289-p102">**Pastaba**: jei anksčiau naudojote IP arba URL leidyba per HTML, XML, ir RSS galinio punkto naujinimų, jūs taip pat turi pereiti prie naujų interneto paslaugų automatizavimo šių tipų naujinimus. Norėdami gauti daugiau informacijos, peržiūrėkite ["Office 365" galinio punkto kategorijos ir Office 365 IP adresą ir URL interneto paslaugos](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="57289-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

