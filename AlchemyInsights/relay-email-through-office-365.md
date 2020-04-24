---
title: Perdavimas el. paštu per „Microsoft 365“
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785203"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="4ad4a-102">Daugiafunkcio įrenginio arba programos, skirtos siųsti el. laiškus, nustatymas</span><span class="sxs-lookup"><span data-stu-id="4ad4a-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="4ad4a-103">Jei norite sužinoti apie galimas parinktis ir veiksmus, žr. [Kaip nustatyti daugiafunkcį įrenginį arba programą siųsti el. laiškus naudojant „Microsoft 365“](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="4ad4a-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="4ad4a-104">**Pastaba:** jei turite įrenginį arba taikomąją programą, kurie neseniai nustojo veikti, atkreipkite dėmesį, kad mes neseniai, kaip planuota, pradėjome [išjungti 3DES šifravimą](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="4ad4a-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="4ad4a-105">Norėdami peržiūrėti susijusius įrenginius, eikite į [SMTP autentifikavimo klientų ataskaitą](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4ad4a-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="4ad4a-106">Dažnai pasitaikančios klaidos gali būti panašios į tokias: autentifikavimo triktis / klaida, TLS triktis / klaida, šifravimo algoritmo neatitikimas, ryšio praradimas.</span><span class="sxs-lookup"><span data-stu-id="4ad4a-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="4ad4a-107">Norėdami išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="4ad4a-107">To resolve the issue:</span></span>
 - <span data-ttu-id="4ad4a-108">**„Windows Server 2003“ IIS SMTP daugiau nebeveiks – reikalinga naujesnė „Windows“ versija.**</span><span class="sxs-lookup"><span data-stu-id="4ad4a-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="4ad4a-109">Patikrinkite savo programoje ar susisiekę su įrenginio tiekėju, ar palaikomas šiuolaikiškas šifras, o galbūt yra naujinimas.</span><span class="sxs-lookup"><span data-stu-id="4ad4a-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
