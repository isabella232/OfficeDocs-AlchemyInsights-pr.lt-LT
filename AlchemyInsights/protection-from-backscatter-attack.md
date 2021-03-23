---
title: Apsauga nuo "backscatter" atakų
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036076"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="2088c-102">Apsauga nuo "backscatter" atakų</span><span class="sxs-lookup"><span data-stu-id="2088c-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="2088c-103">"Backscatter" yra ne pristatymo ataskaitos (taip pat vadinamos NDRs arba peradresavimo pranešimais), kurias gavote už neatsiųstus pranešimus.</span><span class="sxs-lookup"><span data-stu-id="2088c-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="2088c-104">Nepageidaujamo e. pašto platintojus Forge (Spoof) **iš:** savo laiškų adreso, ir jie dažnai naudoja realius elektroninio pašto adresus, kad paskolintų savo laiškus.</span><span class="sxs-lookup"><span data-stu-id="2088c-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="2088c-105">Taigi, kai nepageidaujamo e. pašto platintojus neišvengiamai siunčia laiškus neegzistuojantiems gavėjams, paskirties el. pašto serveris iš esmės apvirsta į nepristatytą pranešimą, esantį NDR su suklastotu siuntėju **iš:** adreso.</span><span class="sxs-lookup"><span data-stu-id="2088c-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="2088c-106">Papildomą informaciją galima rasti " [backscatter" "UOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)".</span><span class="sxs-lookup"><span data-stu-id="2088c-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="2088c-107">**"Backscatter" apsaugos įjungimas**</span><span class="sxs-lookup"><span data-stu-id="2088c-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="2088c-108">Norėdami įjungti "backscatter" apsaugą, atlikite toliau nurodytą kelią.</span><span class="sxs-lookup"><span data-stu-id="2088c-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="2088c-109">**Protection.Office.com > grėsmių valdymo > strategija > Antispam > pasirinkite pašto šiukšlių filtravimo strategiją ir redaguoti strategiją > pašto šiukšlių ypatybės > pažymėti kaip šlamštą > NDR Atgalinės > nustatykite ją "įjungta"**</span><span class="sxs-lookup"><span data-stu-id="2088c-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="2088c-110">Jei manote, kad paskyra buvo pažeista, peržiūrėkite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="2088c-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="2088c-111">Atsakymas į pažeistas el. pašto paskyrą</span><span class="sxs-lookup"><span data-stu-id="2088c-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="2088c-112">Blokuojamų vartotojų pašalinimas iš riboto vartotojų portalo "Office 365"</span><span class="sxs-lookup"><span data-stu-id="2088c-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



