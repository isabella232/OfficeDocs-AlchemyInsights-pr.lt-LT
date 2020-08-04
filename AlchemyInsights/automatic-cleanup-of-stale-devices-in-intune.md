---
title: Automatinis valymas pasenusių prietaisų Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555224"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="f7e8d-102">Automatinis valymas pasenusių prietaisų Intune</span><span class="sxs-lookup"><span data-stu-id="f7e8d-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="f7e8d-103">Intune leidžia administratoriui konfigūruoti laiko intervalą tarp 90 ir 270 dienų, po kurio pasenusi prietaisai pašalinami iš tarnybos.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="f7e8d-104">Šis parametras yra visos organizacijos ir kai aktyvuota įsigalioja iš karto.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="f7e8d-105">Visi įrenginiai, nepažymėti intune serveryje ilgiau nei parametras yra visam laikui panaikinti.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="f7e8d-106">**Pastaba** Šis valymo veiksmas gali būti taikomas tik MDM įrenginio objektams.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="f7e8d-107">EAS neįtraukiami tik įrenginio objektai.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="f7e8d-108">Jei norite gauti papildomos informacijos apie tai, kada įrenginys tampa tinkamas naikinti pagal įrenginio valymo nustatymą ir jo būseną:</span><span class="sxs-lookup"><span data-stu-id="f7e8d-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="f7e8d-109">Nustatymas: **Ištrinti įrenginius po paskutinio įregistravimo datos: Taip (tam tikra vertė (N) nurodytomis dienomis)**</span><span class="sxs-lookup"><span data-stu-id="f7e8d-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="f7e8d-110">Pagal parametre sukonfigūruotą reikšmę (N), "Intune" tarnyba panaikina įrenginį nurodytomis dienomis po paskutinio sėkmingai čekio.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="f7e8d-111">Nustatymas: **ištrinti įrenginius po paskutinės registracijos datos: Ne**</span><span class="sxs-lookup"><span data-stu-id="f7e8d-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="f7e8d-112">Praėjus 180 dienų nuo įrenginio sertifikato galiojimo pabaigos ir jis neatnaujinamas, įrenginys panaikinamas.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="f7e8d-113">**Pastaba** Abiem atvejais įrenginys turi būti sėkmingai užregistruotas Intune.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="f7e8d-114">Registracija įvyksta per pirmąjį įrenginį checkin su Intune paslauga.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="f7e8d-115">Jei įrenginys sėkmingai užregistruoja "Intune", bet netaia ir neužregistravo "Intune", įrenginys panaikinamas praėjus 270 dienų po registracijos.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="f7e8d-116">(90 dienų, kad pažymėtumėte įrenginį kaip atšauktą, o tada dar 180 dienų įrašui panaikinti.)</span><span class="sxs-lookup"><span data-stu-id="f7e8d-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="f7e8d-117">Šiuo metu "Intune" konsolėje nėra mechanizmo, skirto nustatyti įrenginio sertifikavimo galiojimo datą bet kuriam įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="f7e8d-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>