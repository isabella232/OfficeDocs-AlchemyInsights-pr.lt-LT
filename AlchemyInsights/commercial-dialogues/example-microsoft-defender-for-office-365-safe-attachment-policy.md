---
title: "\"Microsoft Defender\", skirtas \"Office 365\" saugaus priedo strategijai"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749203"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="0ddc7-102">"Microsoft Defender", skirtas "Office 365" saugaus priedo strategijai</span><span class="sxs-lookup"><span data-stu-id="0ddc7-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="0ddc7-103">Šie parametrai leidžia strategiją, vadinamą *nėra delsimų* , iš karto pristatančių pranešimą, tada jie vėl prideda priedų, kai jie nuskaitomi:</span><span class="sxs-lookup"><span data-stu-id="0ddc7-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="0ddc7-104">**Pavadinimas**: nėra delsimo</span><span class="sxs-lookup"><span data-stu-id="0ddc7-104">**Name**: No delays</span></span>
- <span data-ttu-id="0ddc7-105">**Aprašas**: iškart pateikia pranešimą ir perteikia priedus.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="0ddc7-106">**Atsakymas**: pasirinkite **dinaminio pristatymo** parinktį.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="0ddc7-107">Daugiau informacijos ieškokite [dinaminio pristatymo saugos priedų strategijose](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="0ddc7-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="0ddc7-108">**Peradresavimo priedo** sekcija: pasirinkite parinktį, kad **įgalintumėte peradresavimą**, tada įveskite savo "Microsoft" 365 visuotinio administratoriaus, saugos administratoriaus arba saugos analitiko, kuris ištirs kenkėjiškus priedus, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="0ddc7-109">**Taikoma** skyriui: pasirinkite **gavėją**, tada pasirinkite savo domeną.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="0ddc7-110">Pasirinkite **įtraukti**, tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="0ddc7-111">Baigę pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="0ddc7-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="0ddc7-112">Norėdami sužinoti daugiau, skaitykite ["Microsoft Defender" saugos priedai, skirti "Office 365"](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="0ddc7-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
