---
title: S/MIME programoje "Outlook" žiniatinklyje
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666848"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="3b46e-102">Užšifruoti el. laiškus "Outlook"</span><span class="sxs-lookup"><span data-stu-id="3b46e-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="3b46e-103">Office 365 pranešimų šifravimas yra pastatytas ant Microsoft Azure teisių valdymo (Azure RMS), kuris yra Azure informacijos apsaugos dalis.</span><span class="sxs-lookup"><span data-stu-id="3b46e-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="3b46e-104">Jei jūsų prenumeratoje yra "Azure" teisių valdymas arba "Azure" informacijos apsauga, **jums nereikia imtis jokių veiksmų, kad įgalintumėte arba suaktyvintumėte** teisių valdymo tarnybą.</span><span class="sxs-lookup"><span data-stu-id="3b46e-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="3b46e-105">Atsižvelgiant į klientų atsiliepimus, mes nebebus įgalinti Exchange pašto srauto taisyklės automatiškai užšifruoti siunčiamų el. laiškų, kuriuose yra tam tikros rūšies slaptą informaciją savo nuomotojo pagal numatytuosius parametrus.</span><span class="sxs-lookup"><span data-stu-id="3b46e-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="3b46e-106">Vietoj to, mes pateikti išsamias instrukcijas apie tai, kaip jūs galite padaryti patys.</span><span class="sxs-lookup"><span data-stu-id="3b46e-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="3b46e-107">Daugiau informacijos, kaip sukurti transportavimo taisyklę slaptai informacijai užšifruoti, rasite [šiame straipsnyje](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="3b46e-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="3b46e-108">Jei naudojate "Outlook" internete (anksčiau **OWA**): kurdami el. laišką, tiesiog spustelėkite **apsaugoti** OWA.</span><span class="sxs-lookup"><span data-stu-id="3b46e-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="3b46e-109">Tai bus taikoma "neperduoti" leidimo.</span><span class="sxs-lookup"><span data-stu-id="3b46e-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="3b46e-110">Spustelėkite **keisti leidimą** ir pasirinkite **šifruoti** , kad užšifruotumėte tik pranešimą.</span><span class="sxs-lookup"><span data-stu-id="3b46e-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="3b46e-111">Jei naudojate **"Outlook Client"**: siųsti užšifruotą pranešimą iš "Outlook" 2013 arba 2016, arba "Outlook" 2016 for Mac, pasirinkite **parinkčių** > **teisės**, tada pasirinkite norimą apsaugos parinktį.</span><span class="sxs-lookup"><span data-stu-id="3b46e-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="3b46e-112">Norėdami **automatiškai užšifruoti visus el. laiškus** , nusiųstus tam tikriems gavėjams arba išorinėms partnerių organizacijoms, turite sukurti pašto srauto transportavimo taisyklę "Exchange" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="3b46e-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="3b46e-113">Išsamios instrukcijos pateikiamos [šiame palaikymo straipsnyje](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="3b46e-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

