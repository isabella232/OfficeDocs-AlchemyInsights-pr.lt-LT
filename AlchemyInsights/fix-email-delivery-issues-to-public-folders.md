---
title: Pašto pristatymo problemų sprendimas pašto viešuosiuose aplankuose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677936"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="b83a3-102">Pašto pristatymo problemų sprendimas pašto viešuosiuose aplankuose</span><span class="sxs-lookup"><span data-stu-id="b83a3-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="b83a3-103">Jei išoriniai siuntėjai negali siųsti laiškų į jūsų pašto viešąjį aplanką, o siuntėjams pateikiama klaida: **nepavyko rasti (550 5.4.1)**, patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip vidinis perdavimo domenas, o ne kaip patikimas domenas:</span><span class="sxs-lookup"><span data-stu-id="b83a3-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="b83a3-104">Atidarykite " [Exchange" administravimo centrą (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="b83a3-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="b83a3-105">Eikite į **pašto srauto** \> **pripa ̨inti domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.</span><span class="sxs-lookup"><span data-stu-id="b83a3-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="b83a3-106">Atsidariusiame ypatybių puslapyje, jei domeno tipas nustatytas kaip **patikimas**, pakeiskite reikšmę į **Vidinė relė** ir spustelėkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="b83a3-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="b83a3-107">Jei išoriniai siuntėjai gauna klaidą, neturite **teisių (550 5.7.13)**, " [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) " "PowerShell" vykdykite šią komandą, kad pamatytumėte anoniminių vartotojų teises viešajame aplanke:</span><span class="sxs-lookup"><span data-stu-id="b83a3-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="b83a3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="b83a3-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="b83a3-109">Norėdami leisti išoriniams vartotojams siųsti laiškus į šį viešąjį aplanką, įtraukite "CreateItems" prieigą prie vartotojo anoniminių.</span><span class="sxs-lookup"><span data-stu-id="b83a3-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="b83a3-110">Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="b83a3-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
