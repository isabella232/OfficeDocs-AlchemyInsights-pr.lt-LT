---
title: Reikia pažymėti domeną arba el. pašto siuntėją?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281179"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="24583-102">Reikia pažymėti domeną arba el. pašto siuntėją?</span><span class="sxs-lookup"><span data-stu-id="24583-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="24583-103">Nerekomenduojama naudoti **saugių siuntėjų sąrašų,** nes ji atveria jūsų organizaciją pašto šiukšlių, fagų ir apsimestinių išpuolių.</span><span class="sxs-lookup"><span data-stu-id="24583-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="24583-104">Tačiau, jei yra verslo poreikis, **rekomenduojame** naudoti **[pašto srauto taisykles.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="24583-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="24583-105">Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (patikrina, ar siuntimo domenas nėra apsimesti).</span><span class="sxs-lookup"><span data-stu-id="24583-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="24583-106">**Pastaba:** nerekomenduojame tvarkyti klaidingų teigiamų rezultatų naudojant patikimų siuntėjų sąrašus, nes pašto šiukšlių filtravimo išimtys gali atidaryti jūsų organizaciją saugos atakoms.</span><span class="sxs-lookup"><span data-stu-id="24583-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="24583-107">Jei jūsų vartotojas (-ai) gauna pranešimus, neteisingai pažymėtus kaip pašto šiukšles arba nepageidaujamą el. paštą, **[praneškite apie pranešimus ir failus "Microsoft".](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="24583-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="24583-108">Reikia **vengti** patikimų siuntėjų programoje "Outlook", leidžiamų siuntėjų sąrašo arba leidžiamų domenų sąrašo apsaugos nuo pašto šiukšlių strategijose, nes siuntėjai apeina visus šlamšto, apgaulės ir apsaugos nuo spaudos ir siuntėjo autentifikavimo (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="24583-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="24583-109">Šis metodas geriausiai tinka tik laikinam bandymui.</span><span class="sxs-lookup"><span data-stu-id="24583-109">This method is best used for temporary testing only.</span></span>
