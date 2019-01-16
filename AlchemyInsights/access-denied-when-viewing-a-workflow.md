---
title: Prieiga uždrausta peržiūrint darbo eigą
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301399"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="19f3b-102">Prieiga uždrausta peržiūrint darbo eigą</span><span class="sxs-lookup"><span data-stu-id="19f3b-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="19f3b-103">SharePoint 2013 darbo eigos, kurios bando siųsti el. laišką SharePoint grupei gali nepavykti su klaidos pranešimą "Prieiga uždrausta" Jei SharePoint grupės narius nustatytas visiems.</span><span class="sxs-lookup"><span data-stu-id="19f3b-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="19f3b-104">**Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:**</span><span class="sxs-lookup"><span data-stu-id="19f3b-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="19f3b-105">Leisti visiems matyti SharePoint grupės nariai.</span><span class="sxs-lookup"><span data-stu-id="19f3b-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="19f3b-106">Pašalinti SharePoint grupę iš kam arba kopija el. linija.</span><span class="sxs-lookup"><span data-stu-id="19f3b-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="19f3b-107">Tiesiogiai pridėti vartotojus prie kam arba kopija line, jei SharePoint grupės narystės matomumo keisti negalima.</span><span class="sxs-lookup"><span data-stu-id="19f3b-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="19f3b-108">Norėdami peržiūrėti daugiau informacijos prašome kreiptis į [HTTP neleistina į /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="19f3b-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

