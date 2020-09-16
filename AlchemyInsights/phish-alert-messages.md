---
title: "\"2491\" įspėjimų el. laiškai iš \"Phish\", pateiktos dėl nuomotojo arba vartotojo perrašymo strategijos"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728619"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="9583f-102">Įspėjimų el. laiškai iš "Phish", pateiktos dėl nuomotojo arba vartotojo perrašymo strategijos</span><span class="sxs-lookup"><span data-stu-id="9583f-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="9583f-103">Numatytoji įspėjimų politika, pavadinta "Phish, pateikta dėl nuomotojo arba vartotojo nepaisymo", buvo išskleista nuomininkams su "Office 365" ATP P1 ir P2 licencijomis.</span><span class="sxs-lookup"><span data-stu-id="9583f-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="9583f-104">Jei gavote šį įspėjimą, atlikite veiksmus, skirtus tyrimui:</span><span class="sxs-lookup"><span data-stu-id="9583f-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="9583f-105">Įspėjimo pranešime spustelėkite **Peržiūrėti įspėjimą** , kad pereitumėte į **įspėjimų** puslapį saugos & atitikties centre.</span><span class="sxs-lookup"><span data-stu-id="9583f-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="9583f-106">Pasirinkite įspėjimą, kad matytumėte parinktį **Peržiūrėti pranešimų sąrašą** arba **peržiūrėti pranešimus programoje "Explorer"**.</span><span class="sxs-lookup"><span data-stu-id="9583f-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="9583f-107">Abi šios parinktys padės jums pateikti pranešimo informaciją, kuri apima pranešimo ID.</span><span class="sxs-lookup"><span data-stu-id="9583f-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="9583f-108">Žinokite, kad saitas Threat Explorer automatiškai filtruos pranešimus, atitinkančius įspėjimų kriterijus.</span><span class="sxs-lookup"><span data-stu-id="9583f-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="9583f-109">Gali reikėti pakoreguoti datos filtrą grėsmių naršyklėje.</span><span class="sxs-lookup"><span data-stu-id="9583f-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="9583f-110">Apsimestinis laiškas buvo pristatytas dėl neautomatiniu būdu sukonfigūruotos perrašymo:</span><span class="sxs-lookup"><span data-stu-id="9583f-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="9583f-111">Vartotojo nustatytas leistinas siuntėjas arba domenas.</span><span class="sxs-lookup"><span data-stu-id="9583f-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="9583f-112">"Anti-spam" strategijos administratorius nustato leidžiamą siuntėjo arba domeno.</span><span class="sxs-lookup"><span data-stu-id="9583f-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="9583f-113">Leidžiamas IP adresas ryšių filtro strategijoje.</span><span class="sxs-lookup"><span data-stu-id="9583f-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="9583f-114">Pašto srauto taisyklė (dar vadinama transportavimo taisykle), sukonfigūruota leisti laiškus.</span><span class="sxs-lookup"><span data-stu-id="9583f-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="9583f-115">Jei manote, kad laiškas klaidingai pažymėtas kaip "Phish", naudokite "Outlook" [ataskaitos pranešimo papildinį](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) , kad pateiktumėte laiškų pavyzdžius "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="9583f-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
