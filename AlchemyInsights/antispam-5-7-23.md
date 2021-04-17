---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821419"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="5d858-102">El. pašto pristatymo problemų sprendimas dėl klaidos kodo 5.7.23</span><span class="sxs-lookup"><span data-stu-id="5d858-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="5d858-103">Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintoją žiniatinklyje.</span><span class="sxs-lookup"><span data-stu-id="5d858-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="5d858-104">Patikrinkite, ar "Microsoft" neįvardifikuoja siunčiamo pranešimo kaip pašto šiukšlių ir nukreipiamas per [didelės rizikos pristatymo telkinį.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="5d858-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="5d858-105">Pranešimai didelės rizikos pristatymo telkinyje neišduos SPF patikrų, todėl paskirties el. pašto organizacija jų nepriims.</span><span class="sxs-lookup"><span data-stu-id="5d858-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="5d858-106">Jei problema išlieka, gali tekti kreiptis į pašto pagrindinio kompiuterio, į kurį bandote siųsti el. paštą, administratorių.</span><span class="sxs-lookup"><span data-stu-id="5d858-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="5d858-107">Atkreipkite dėmesį į išsamią išorinę klaidą, galimų atmetimo pranešime.</span><span class="sxs-lookup"><span data-stu-id="5d858-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="5d858-108">"Microsoft" palaikymas gali nepadėti toliau.</span><span class="sxs-lookup"><span data-stu-id="5d858-108">Microsoft support may not be able to assist further.</span></span>
