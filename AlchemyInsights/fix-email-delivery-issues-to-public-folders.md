---
title: El. pašto pristatymo problemų sprendimas į pašto viešųjų aplankų
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752678"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="98af6-102">El. pašto pristatymo problemų sprendimas į pašto viešųjų aplankų</span><span class="sxs-lookup"><span data-stu-id="98af6-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="98af6-103">Jei Išoriniams siuntėjams negali siųsti pranešimus į savo pašto viešųjų aplankų ir siuntėjų gauti klaidos pranešimą: **nepavyko rasti (550 5.4.1)**, patikrinkite el. pašto domeno, nes viešasis aplankas yra sukonfigūruotas kaip vidinis perdavimo domenas, o ne su patikimą domeną:</span><span class="sxs-lookup"><span data-stu-id="98af6-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="98af6-104">Atidaryti [Exchange administravimo centro (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="98af6-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="98af6-105">Eikite į **pašto srautą** \> **priimta domenai**, pasirinkite pripažintą domeną, ir tada spustelėkite **Redaguoti**.</span><span class="sxs-lookup"><span data-stu-id="98af6-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="98af6-106">Ypatybės, atveriamas, jei domeno tipas yra nustatytas kaip **Authoritative**, reikšmę pakeiskite į **vidaus perdavimo** ir tada spustelėkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="98af6-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="98af6-107">Jei išorinių siuntėjų gauti klaidos, **jūs neturite teisės (550 5.7.13)**, vykdykite šią komandą į [Exchange Online "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) Norėdami matyti, kokias teises anoniminiams vartotojams viešajame aplanke:</span><span class="sxs-lookup"><span data-stu-id="98af6-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="98af6-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="98af6-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="98af6-109">Išorės vartotojai gali siųsti laišką į šį viešąjį aplanką, pridėti CreateItems prieigos teisę į anoniminis vartotojas.</span><span class="sxs-lookup"><span data-stu-id="98af6-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="98af6-110">Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="98af6-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
