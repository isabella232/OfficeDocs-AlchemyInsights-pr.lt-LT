---
title: SMTP autentifikavimo problemų sprendimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826423"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="6a139-102">SMTP autentifikavimo problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="6a139-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="6a139-103">Jei gaunate 5.7.57 arba 5.7.3 klaidų bandydami siųsti SMTP el. paštą ir autentifikuoti naudodami klientą arba taikomąją programą, yra keletas dalykų, kuriuos turėtumėte patikrinti:</span><span class="sxs-lookup"><span data-stu-id="6a139-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="6a139-104">Autentifikuotas SMTP pateikimas gali būti išjungtas jūsų nuomotoje arba pašto dėžutėje, kurią bandote naudoti (patikrinkite abu parametrus).</span><span class="sxs-lookup"><span data-stu-id="6a139-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="6a139-105">Norėdami skaityti daugiau, žr. [Autentifikuoto kliento SMTP pateikimo įjungimas arba išjungimas](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="6a139-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="6a139-106">Patikrinkite, [ar jūsų nuomotojui įgalintos "Azure"](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) saugos numatytosios funkcijos; jei įgalinta, SMTP autentifikavimas naudojant bazinį autentifikavimą (dar vadinamą senesniu; bus naudojamas vartotojo vardas ir slaptažodis) nepavyks.</span><span class="sxs-lookup"><span data-stu-id="6a139-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
