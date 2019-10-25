---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682216"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="aef3f-102">FIX el. pašto pristatymo problemos klaidos kodas 5.7.23</span><span class="sxs-lookup"><span data-stu-id="aef3f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="aef3f-103">Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintuve žiniatinklyje.</span><span class="sxs-lookup"><span data-stu-id="aef3f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="aef3f-104">Patikrinkite, ar siunčiamojo laiško nebuvo nustatyta kaip šlamštas Office 365 ir nukreipiami per [didelis rizikos pristatymo telkinys](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="aef3f-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="aef3f-105">Didelės rizikos pristatymo telkinio pranešimai nepraeis SPF patikros, todėl paskirties el. pašto organizacijos nepriims.</span><span class="sxs-lookup"><span data-stu-id="aef3f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="aef3f-106">Jei problema kartojasi, jums gali tekti susisiekti su pašto serverio, į kurį bandote siųsti el. laišką, administratoriumi.</span><span class="sxs-lookup"><span data-stu-id="aef3f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="aef3f-107">Užsirašykite išsamią išorinę klaidą peradresavimo pranešime.</span><span class="sxs-lookup"><span data-stu-id="aef3f-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="aef3f-108">Office 365 parama gali nepavykti toliau.</span><span class="sxs-lookup"><span data-stu-id="aef3f-108">Office 365 support may not be able to assist further.</span></span>