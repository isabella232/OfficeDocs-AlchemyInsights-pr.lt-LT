---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717333"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="2a40f-102">Klaidos kodo 5.7.23. pašto pristatymo problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="2a40f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="2a40f-103">Patikrinkite savo domeno SPF DNS įrašą viešai prieinamame SPF arba DNS įrašų tikrintuve žiniatinklyje.</span><span class="sxs-lookup"><span data-stu-id="2a40f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="2a40f-104">Patikrinkite, ar siuntimo laiškas nebuvo identifikuojamas kaip šlamštas "Microsoft" ir nukreipiamas per [didelės rizikos pristatymo telkinį](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="2a40f-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="2a40f-105">Didelės rizikos pristatymo telkinio laiškai nepereis SPF, todėl nebus priimami paskirties el. pašto organizacija.</span><span class="sxs-lookup"><span data-stu-id="2a40f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="2a40f-106">Jei problema kartojasi, jums gali tekti kreiptis į pašto pagrindinio kompiuterio, kuriam bandote siųsti laišką, administratorių.</span><span class="sxs-lookup"><span data-stu-id="2a40f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="2a40f-107">Užsirašykite išsamią išorinę klaidą, esančią peradresavimo pranešime.</span><span class="sxs-lookup"><span data-stu-id="2a40f-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="2a40f-108">"Microsoft" palaikymo tarnyba gali būti nepajėgi toliau padėti.</span><span class="sxs-lookup"><span data-stu-id="2a40f-108">Microsoft support may not be able to assist further.</span></span>
