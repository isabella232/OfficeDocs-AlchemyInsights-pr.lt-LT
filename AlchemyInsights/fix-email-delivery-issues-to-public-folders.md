---
title: El. pašto pristatymo problemų sprendimas viešuosiuose aplankuose, kuriuose įgalintas paštas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716360"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="e370e-102">El. pašto pristatymo problemų sprendimas viešuosiuose aplankuose, kuriuose įgalintas paštas</span><span class="sxs-lookup"><span data-stu-id="e370e-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="e370e-103">Jei išoriniai siuntėjai negali siųsti pranešimų į jūsų pašto viešuosius aplankus, o siuntėjai gauna klaidą: **nepavyko rasti (550 5.4.1),** patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip vidinis perdavimo domenas, o ne patikimas domenas:</span><span class="sxs-lookup"><span data-stu-id="e370e-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="e370e-104">Atidarykite ["Exchange" administravimo centrą (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="e370e-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="e370e-105">Eikite į **Pašto srautas** \> **Pripažinti domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.</span><span class="sxs-lookup"><span data-stu-id="e370e-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="e370e-106">Atsidariusiame ypatybių puslapyje, jei domeno tipas nustatytas kaip **Patikimas**, pakeiskite reikšmę į **Vidinis perdavimas,** tada spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="e370e-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="e370e-107">Jei išoriniai siuntėjai gauna **klaidą, jūs neturite teisių (550 5.7.13),** vykdykite šią komandą Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) norėdami pamatyti anoniminių vartotojų teises viešajame aplanke:</span><span class="sxs-lookup"><span data-stu-id="e370e-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="e370e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Pavyzd3/4iui, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="e370e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="e370e-109">Norėdami leisti išoriniams vartotojams siųsti el. laiškus į šį viešąjį aplanką, įtraukite CreateItems prieigą tiesiai vartotojui Anonimas.</span><span class="sxs-lookup"><span data-stu-id="e370e-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="e370e-110">Pavyzd3/4iui, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="e370e-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
