---
title: 1554 Winsock klaida 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419988"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="01809-102">Winsock klaida 10061</span><span class="sxs-lookup"><span data-stu-id="01809-102">Winsock error 10061</span></span>

<span data-ttu-id="01809-103">Ši klaida reiškia, kad "Office 365" negalėjo sukurti TCP socket (jungtis) su tikslinės priimančiosios.</span><span class="sxs-lookup"><span data-stu-id="01809-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="01809-104">Labiausiai tikėtina, dažniausia šios klaidos priežastis yra ugniasienės konfigūracijos problema.</span><span class="sxs-lookup"><span data-stu-id="01809-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="01809-105">Norėdami išspręsti šią problemą, patikrinkite šiuos parametrus:</span><span class="sxs-lookup"><span data-stu-id="01809-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="01809-106">Patikrinkite, ar jūsų ugniasienės konfigūracijos informacija iš [Office 365 URL ir IP adresų diapazonas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="01809-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="01809-107">Jei klaidos yra susijusios su Exchange Online Protection (EOP), jums turėtų anksčiau pranešama apie pasikeičia į [Exchange Online apsaugos IP adresus](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="01809-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="01809-108">Įsitikinkite, kad jūsų interneto paslaugų teikėjas (ISP) neblokuoja uosto.</span><span class="sxs-lookup"><span data-stu-id="01809-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="01809-109">Patikrinkite, ar protingas pagrindinio kompiuterio ir paskirties serverio parametrus jūsų jungtys.</span><span class="sxs-lookup"><span data-stu-id="01809-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="01809-110">Atkreipkite dėmesį, kad "Office 365" ne blokuoti *priimamus* ryšius, tokiu būdu.</span><span class="sxs-lookup"><span data-stu-id="01809-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
