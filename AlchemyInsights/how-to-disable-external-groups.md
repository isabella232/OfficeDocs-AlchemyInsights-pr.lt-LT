---
title: Kaip išjungti išorinės grupės
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384833"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="e3027-102">Kaip išjungti išorinės grupės</span><span class="sxs-lookup"><span data-stu-id="e3027-102">How to disable External Groups</span></span>

<span data-ttu-id="e3027-103">"Yammer" išoriniai pranešimai taikoma Exchange transportavimo taisykles (ETRs), užkirsti kelią įmonės informacijos bendrinimą iniciatyvus valdiklių rinkinys.</span><span class="sxs-lookup"><span data-stu-id="e3027-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="e3027-104">Siekiant apriboti vartotojams iš užsienio grupių kūrimas, turite konfigūruoti Exchange transportavimo taisyklės (toliau – ETR), ir tada konfigūruoti "Yammer" naudoti Exchange transportavimo taisyklė blokuoti išoriniai pranešimai.</span><span class="sxs-lookup"><span data-stu-id="e3027-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="e3027-105">Kai sukuriate taisyklę Exchange Online administravimo centrą, atlikite šiuos veiksmus nustatyti ETR galimybę kreiptis į "Yammer":</span><span class="sxs-lookup"><span data-stu-id="e3027-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="e3027-106">Prisijungti prie "Yammer" viešėjusių admin, ir **"Yammer" administravimo centrą**, pereikite prie C **turinio ir saugumo \> securitysettings.**</span><span class="sxs-lookup"><span data-stu-id="e3027-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="e3027-107">**Išoriniai pranešimai**pasirinkite **vykdyti jūsų Exchange Online Exchange transportavimo taisykles (ETRs), "Yammer".**</span><span class="sxs-lookup"><span data-stu-id="e3027-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="e3027-108">Pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="e3027-108">Choose **Save**.</span></span>

<span data-ttu-id="e3027-109">Daugiau informacijos rasite [valdymo išorės pranešimus "Yammer" tinkle su Exchange transportavimo taisyklės](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="e3027-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  