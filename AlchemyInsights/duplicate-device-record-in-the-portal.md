---
title: Pasikartojantis įrenginio įrašas portale
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814524"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="fc0d0-102">Pasikartojantis įrenginio įrašas portale</span><span class="sxs-lookup"><span data-stu-id="fc0d0-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="fc0d0-103">Galite matyti 2 įrenginio įrašus portale, jei įrenginys netinkamai praneša apie bendro valdymo būseną į Konfigūracijos tvarkyklės svetainę.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="fc0d0-104">Norėdami patikrinti įrenginio bendro valdymo būseną, peržiūrėkite **bendrai valdomo įrenginio** stulpelį Konfigūracijos tvarkyklės konsolėje.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="fc0d0-105">Jei stulpelis nerodomas, galite jį įtraukti dešiniuoju pelės klavišu spustelėdami bet kurią stulpelio antraštę ir pažymėdami jį sąraše.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="fc0d0-106">Bendrai valdoma reikšmė turi būti **Taip**.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="fc0d0-107">Jei reikšmė yra **Ne**, atidarykite Konfigūracijos tvarkyklės kliento programą kliento įrenginyje ir skirtuke Bendra pažymėkite ypatybę **Bendras valdymas**.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="fc0d0-108">Jei reikšmė **Įgalinta**, tai reiškia problemas su kliento ir valdymo taško ryšiu.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="fc0d0-109">Peržiūrėkite **CcmMessaging.log** įrenginyje, kad ištirtumėte galimas ryšio triktis.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="fc0d0-110">Jei reikšmė **Išjungta** ir įrenginys užregistruotas „Intune“, įsitikinkite, kad įrenginys gavo bendro valdymo strategiją peržiūrę **CoManagementHandler. log** įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="fc0d0-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
