---
title: Apsaugos nuo brukalo - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676505"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="83ce2-102">El. pašto pristatymo problemų sprendimas klaidos kodas 5.7.23</span><span class="sxs-lookup"><span data-stu-id="83ce2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="83ce2-103">Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintuve žiniatinklyje.</span><span class="sxs-lookup"><span data-stu-id="83ce2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="83ce2-104">Patikrinkite, ar "Microsoft" nenustatė siunčiamo pranešimo kaip pašto šiukšlių ir nurodė per [didelės rizikos pristatymo telkinį](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="83ce2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="83ce2-105">Didelės rizikos pristatymo telkinio pranešimai neišlaikys SPF patikrinimų, todėl paskirties el. pašto organizacija jų nepriims.</span><span class="sxs-lookup"><span data-stu-id="83ce2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="83ce2-106">Jei problema išlieka, gali tekti susisiekti su pašto pagrindinio kompiuterio, į kurį bandote siųsti el. laiškus, administratoriumi.</span><span class="sxs-lookup"><span data-stu-id="83ce2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="83ce2-107">Užsirašykite išsamią išorinę klaidą, pasiekiamą atmetimo pranešime.</span><span class="sxs-lookup"><span data-stu-id="83ce2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="83ce2-108">"Microsoft" palaikymo tarnyba gali negalėti toliau padėti.</span><span class="sxs-lookup"><span data-stu-id="83ce2-108">Microsoft support may not be able to assist further.</span></span>
