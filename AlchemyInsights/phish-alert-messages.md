---
title: 2491 Įspėjimo el. laiškus iš "Phish pristatytas dėl nuomotojo arba vartotojo nepaisyti" strategija
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758936"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="d1943-102">Įspėjimo el. laiškus iš "Phish pristatytas dėl nuomotojo arba vartotojo nepaisyti" strategija</span><span class="sxs-lookup"><span data-stu-id="d1943-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="d1943-103">Numatytoji įspėjimo strategija, pavadinta "Phish Delivered dėl nuomotojo arba vartotojo nepaisyti" buvo iškočiojama nuomininkams su "Office 365" ATP P1 ir P2 licencijomis.</span><span class="sxs-lookup"><span data-stu-id="d1943-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="d1943-104">Jei gavote šį įspėjimą, toliau pateikiami veiksmai, kuriuos reikia ištirti.</span><span class="sxs-lookup"><span data-stu-id="d1943-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="d1943-105">Įspėjimo pranešime spustelėkite **Peržiūrėti įspėjimą,** kad pereitumėte į saugos & atitikties centro puslapį **Įspėjimai.**</span><span class="sxs-lookup"><span data-stu-id="d1943-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="d1943-106">Pasirinkite įspėjimą, kad pamatytumėte parinktį **Peržiūrėti pranešimų sąrašą** arba **Peržiūrėti pranešimus naršyklėje**.</span><span class="sxs-lookup"><span data-stu-id="d1943-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="d1943-107">Abi šios parinktys nuves jus prie pranešimo išsamios informacijos, kurioje yra pranešimo ID.</span><span class="sxs-lookup"><span data-stu-id="d1943-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="d1943-108">Atminkite, kad threat explorer saitas automatiškai filtruoja pranešimus, atitinkančius įspėjimo kriterijus.</span><span class="sxs-lookup"><span data-stu-id="d1943-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="d1943-109">Gali tekti koreguoti datos filtrą "Threat Explorer".</span><span class="sxs-lookup"><span data-stu-id="d1943-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="d1943-110">Apsimestinių svetainių pranešimas buvo pristatytas dėl neautomatiniu būdu sukonfigūruoto nepaisymo:</span><span class="sxs-lookup"><span data-stu-id="d1943-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="d1943-111">Vartotojo nustatytas leidžiamas siuntėjas arba domenas.</span><span class="sxs-lookup"><span data-stu-id="d1943-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="d1943-112">Leidžiamas siuntėjas arba domenas, kurį administratorius nustato apsaugos nuo pašto šiukšlių politikoje.</span><span class="sxs-lookup"><span data-stu-id="d1943-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="d1943-113">Leidžiamas IP adresas ryšio filtro strategijoje.</span><span class="sxs-lookup"><span data-stu-id="d1943-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="d1943-114">Pašto srauto taisyklė (dar vadinama transportavimo taisykle), sukonfigūruota leisti pranešimus.</span><span class="sxs-lookup"><span data-stu-id="d1943-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="d1943-115">Jei manote, kad pranešimas buvo neteisingai pažymėtas kaip phish, naudokite "Outlook" [ataskaitų pranešimo papildinį](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) pateikti pranešimų pavyzdžių "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="d1943-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
