---
title: Hibridinės aplinkos pranešimų šifravimo konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526595"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="54c88-102">Hibridinės aplinkos pranešimų šifravimo konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="54c88-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="54c88-103">Jei naudojate hibridinio "Exchange" aplinką, vietiniai vartotojai gali siųsti užšifruotą laišką naudodami "Office" pranešimų šifravimą (OME) tik tuo atveju, jei laiškas nukreipiamas naudojant "Exchange Online"</span><span class="sxs-lookup"><span data-stu-id="54c88-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="54c88-104">Norėdami šifruoti laiškus naudodami OME, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="54c88-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="54c88-105">Naudokite [hibridinio konfigūravimo vediklį](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) , kad nustatytumėte hibridinę aplinką.</span><span class="sxs-lookup"><span data-stu-id="54c88-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="54c88-106">Norint nustatyti šifravimą, nereikia atlikti jokių specialių veiksmų.</span><span class="sxs-lookup"><span data-stu-id="54c88-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="54c88-107">[Nustatykite pašto srauto taisykles šifravimui,](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) kaip įprastai.</span><span class="sxs-lookup"><span data-stu-id="54c88-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


