---
title: Perdavimas el. paštu per „Office 365“
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
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745405"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="2d06f-102">Daugiafunkcio įrenginio arba programos, skirtos siųsti el. laiškus naudojant „Office 365“, nustatymas</span><span class="sxs-lookup"><span data-stu-id="2d06f-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="2d06f-103">Jei norite sužinoti apie galimas parinktis ir veiksmus, žr. [Kaip nustatyti daugiafunkcį įrenginį arba programą siųsti el. laiškus naudojant „Office 365“](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="2d06f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="2d06f-104">**Pastaba:** jei turite įrenginį arba taikomąją programą, kurie neseniai nustojo veikti, atkreipkite dėmesį, kad mes neseniai, kaip planuota, pradėjome [išjungti 3DES šifravimą](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="2d06f-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="2d06f-105">Norėdami peržiūrėti susijusius įrenginius, eikite į [SMTP autentifikavimo klientų ataskaitą](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="2d06f-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="2d06f-106">Dažnai pasitaikančios klaidos gali būti panašios į tokias: autentifikavimo triktis / klaida, TLS triktis / klaida, šifravimo algoritmo neatitikimas, ryšio praradimas.</span><span class="sxs-lookup"><span data-stu-id="2d06f-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="2d06f-107">Norėdami išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="2d06f-107">To resolve the issue:</span></span>
 - <span data-ttu-id="2d06f-108">**„Windows Server 2003“ IIS SMTP daugiau nebeveiks – reikalinga naujesnė „Windows“ versija.**</span><span class="sxs-lookup"><span data-stu-id="2d06f-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="2d06f-109">Patikrinkite savo programoje ar susisiekę su įrenginio tiekėju, ar palaikomas šiuolaikiškas šifras, o galbūt yra naujinimas.</span><span class="sxs-lookup"><span data-stu-id="2d06f-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
