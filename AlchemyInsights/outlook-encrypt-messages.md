---
title: S/MIME "Outlook" žiniatinklyje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772306"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="3e11c-102">El. laiškų šifravimas programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="3e11c-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="3e11c-103">"Microsoft 365" pranešimų šifravimas yra sukurtas "Microsoft Azure Rights Management" ("Azure RMS"), kuris yra "Azure" informacijos apsaugos dalis.</span><span class="sxs-lookup"><span data-stu-id="3e11c-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="3e11c-104">Jei jūsų produktų pakete yra "Azure Rights Management" arba "Azure" informacijos apsauga, **jums nereikia imtis jokių veiksmų, kad rankiniu būdu įgalintumėte arba suaktyvintumėte** teisių valdymo tarnybą.</span><span class="sxs-lookup"><span data-stu-id="3e11c-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="3e11c-105">Atsižvelgdami į klientų atsiliepimus, nebegalėsite įgalinti "Exchange" pašto srauto taisyklių, kad automatiškai šifruotų siunčiamus laiškus, kuriuose yra tam tikro tipo slaptos informacijos pagal numatytuosius reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="3e11c-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="3e11c-106">Vietoj to, mes teikiame išsamias instrukcijas, kaip galite tai padaryti patys.</span><span class="sxs-lookup"><span data-stu-id="3e11c-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="3e11c-107">Daugiau informacijos apie tai, kaip sukurti transportavimo taisyklę, kad užšifruotų slaptą informaciją, rasite [šiame straipsnyje](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="3e11c-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="3e11c-108">Jei naudojate "Outlook" žiniatinklyje (anksčiau **OWA**): kurdami el. laišką, tiesiog spustelėkite **apsaugoti** OWA.</span><span class="sxs-lookup"><span data-stu-id="3e11c-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="3e11c-109">Tai bus taikoma "Nepersiųskite" leidimo.</span><span class="sxs-lookup"><span data-stu-id="3e11c-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="3e11c-110">Spustelėkite **Keisti teises** ir pasirinkite **šifruoti** , kad būtų šifruojamas tik pranešimas.</span><span class="sxs-lookup"><span data-stu-id="3e11c-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="3e11c-111">Jei naudojate **"Outlook Client**": Norėdami nusiųsti šifruotą pranešimą iš "Outlook" 2013 arba "2016" arba "Outlook 2016 for Mac", pasirinkite **parinkčių**  >  **teisės**, tada pasirinkite reikiamą apsaugos parinktį.</span><span class="sxs-lookup"><span data-stu-id="3e11c-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="3e11c-112">Norėdami **automatiškai šifruoti visus el. laiškus** , siunčiamus tam tikriems gavėjams arba išoriniams partnerių organizacijoms, turite sukurti pašto srauto taisyklę "Exchange" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="3e11c-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="3e11c-113">[Šiame palaikymo straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)pateikiamos išsamios instrukcijos.</span><span class="sxs-lookup"><span data-stu-id="3e11c-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

