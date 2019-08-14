---
title: 2491 įspėjimo el. laiškus iš "Phish pareikšta dėl nuomininko ar naudotojo Rankinis valdymas" politikos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391404"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5b524-102">Įspėjimo el. laiškus iš "Phish pareikšta dėl nuomininko ar naudotojo Rankinis valdymas" politikos</span><span class="sxs-lookup"><span data-stu-id="5b524-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5b524-103">Numatytasis įspėjimo strategiją pavadinimu "Phish pristatyta dėl nuomininko ar naudotojo nepaisyti" buvo iškočiojama nuomininkams Office 365 ATP P1 ir P2 licencijas.</span><span class="sxs-lookup"><span data-stu-id="5b524-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="5b524-104">Jei gavote šį perspėjimą, atlikite šiuos veiksmus, siekiant ištirti:</span><span class="sxs-lookup"><span data-stu-id="5b524-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5b524-105">Įspėjimo pranešimas, spustelėkite **Rodyti perspėjimą** eiti į puslapį **įspėjimus** , saugos & atitikties užtikrinimo centre.</span><span class="sxs-lookup"><span data-stu-id="5b524-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5b524-106">Pasirinkite įspėjimo sudaryta galimybė **Peržiūrėti pranešimų sąraše** arba **peržiūrėti pranešimus "Internet Explorer"**.</span><span class="sxs-lookup"><span data-stu-id="5b524-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5b524-107">Abiem nurodytais būdais priimti jus į išsamią informaciją apie pranešimą, kuris apima pranešimą ID.</span><span class="sxs-lookup"><span data-stu-id="5b524-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5b524-108">Atkreipkite dėmesį, kad grėsmių naršyklė nuoroda bus automatiškai filtruoti įspėjimo kriterijus atitinkančius pranešimus.</span><span class="sxs-lookup"><span data-stu-id="5b524-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5b524-109">Reikia pakeisti datos filtras grėsmė "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="5b524-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5b524-110">Sukčiavimo apsimetant pranešimas buvo pristatytas dėl rankiniu būdu konfigūruojami nepaisyti:</span><span class="sxs-lookup"><span data-stu-id="5b524-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5b524-111">Leidžiama siuntėjo ar domeno vartotojo nustatytus.</span><span class="sxs-lookup"><span data-stu-id="5b524-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5b524-112">Dėl leidžiamų siuntėją arba domeną, nustatytą apsaugos nuo pašto šiukšlių strategijos administratorius.</span><span class="sxs-lookup"><span data-stu-id="5b524-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5b524-113">Leidžiamų IP adresą į ryšio filtravimo strategija.</span><span class="sxs-lookup"><span data-stu-id="5b524-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5b524-114">Pašto srautas taisyklę (taip pat žinomas kaip transportavimo taisyklę), sukonfigūruotas leisti pranešimus.</span><span class="sxs-lookup"><span data-stu-id="5b524-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5b524-115">Jei manote, kad pranešimas buvo neteisingai pažymėtas kaip sukčiavimo atvejį, naudokite į "Outlook" [ataskaitos pranešimas papildinys](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) pateikti pranešimą mėginius į "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="5b524-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
