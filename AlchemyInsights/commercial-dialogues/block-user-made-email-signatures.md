---
title: Blokuoti vartotojo sukurtus el. pašto parašus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482309"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="23db0-102">Blokuoti vartotojo sukurtus el. pašto parašus</span><span class="sxs-lookup"><span data-stu-id="23db0-102">Block user-made email signatures</span></span>

<span data-ttu-id="23db0-103">Šis sprendimas taikomas tik el. pašto parašams, sukurtiems internetinėje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="23db0-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="23db0-104">Galite blokuoti parašus tik "Outlook" programoje, jei turite vietinį "Exchange" serverį.</span><span class="sxs-lookup"><span data-stu-id="23db0-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="23db0-105">Administravimo centre pasirinkite **administravimo centrų**  >  **keitimas**.</span><span class="sxs-lookup"><span data-stu-id="23db0-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="23db0-106">Spustelėkite **teisės**  >  **"Outlook Web App" strategijos**.</span><span class="sxs-lookup"><span data-stu-id="23db0-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="23db0-107">Pasirinkite strategiją, tada spustelėkite pieštuko piktogramą, kad jį redaguotumėte.</span><span class="sxs-lookup"><span data-stu-id="23db0-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="23db0-108">Spustelėkite **funkcijos**  >  **daugiau parinkčių**.</span><span class="sxs-lookup"><span data-stu-id="23db0-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="23db0-109">Dalyje **vartotojų veikimas** išvalykite žymės langelį **el. pašto parašas** , tada spustelėkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="23db0-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="23db0-110">**Svarbu:** Jei prieš išvalant šį žymės langelį buvo pridėtas parašas, vartotojas vis tiek galės jį naudoti.</span><span class="sxs-lookup"><span data-stu-id="23db0-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="23db0-111">Paprašykite jų pašalinti.</span><span class="sxs-lookup"><span data-stu-id="23db0-111">Ask them to remove it.</span></span>
