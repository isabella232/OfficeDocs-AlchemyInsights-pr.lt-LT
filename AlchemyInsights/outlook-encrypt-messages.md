---
title: S/MIME internetinėje "Outlook"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511516"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="fe1c9-102">Šifruoti el. Laiškus "Outlook"</span><span class="sxs-lookup"><span data-stu-id="fe1c9-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="fe1c9-103">"Microsoft 365" pranešimų šifravimas yra sukurtas naudojant "Microsoft Azure" teisių valdymą ("Azure RMS"), kuris yra "Azure" informacijos apsaugos dalis.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="fe1c9-104">Jei jūsų prenumerata apima "Azure Rights Management" arba "Azure" informacijos apsaugą, **jums nereikia imtis jokių veiksmų, kad rankiniu būdu įgalintumėte arba suaktyvintumėte** teisių valdymo tarnybą.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="fe1c9-105">Atsižvelgdami į klientų atsiliepimus, nebeleisime Exchange pašto srauto taisyklėms automatiškai užšifruoti siunčiamus el. laiškus, kuriuose yra tam tikro tipo slaptos informacijos jūsų nuomotojo pagal numatytuosius nustatymus.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="fe1c9-106">Vietoj to, mes teikiame išsamias instrukcijas, kaip jūs galite tai padaryti patys.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="fe1c9-107">Papildomos informacijos apie tai, kaip sukurti transportavimo taisyklę slaptai informacijai šifruoti, ieškokite [šiame straipsnyje](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="fe1c9-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="fe1c9-108">Jei naudojate "Outlook" internete (anksčiau **OWA):** kai kuriate el. laišką, tiesiog spustelėkite **apsaugoti** OWA.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="fe1c9-109">Tai bus taikoma "Nepersiųsti" leidimą.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="fe1c9-110">Spustelėkite **Keisti teises** ir pasirinkite **Šifruoti,** kad užšifruotumėte tik pranešimą.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="fe1c9-111">Jei naudojate **"Outlook" klientą**: Norėdami siųsti šifruotą pranešimą iš "Outlook 2013" arba "Outlook 2016 for Mac", pasirinkite **Options**  >  **Parinkčių teisės**, tada pasirinkite reikiamą apsaugos parinktį.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="fe1c9-112">Norėdami **automatiškai užšifruoti visus el. laiškus,** išsiųstus tam tikriems gavėjams arba išorinių partnerių organizacijoms, turite sukurti pašto srauto transportavimo taisyklę "Exchange" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="fe1c9-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="fe1c9-113">Išsamios instrukcijos pateiktos [šiame palaikymo straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="fe1c9-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

