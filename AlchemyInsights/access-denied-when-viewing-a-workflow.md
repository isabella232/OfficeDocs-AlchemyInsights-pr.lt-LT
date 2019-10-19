---
title: Peržiūrint darbo eigą uždrausta prieiga
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747756"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="7c1a7-102">Peržiūrint darbo eigą uždrausta prieiga</span><span class="sxs-lookup"><span data-stu-id="7c1a7-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="7c1a7-103">SharePoint 2013 darbo eigų, bandoma siųsti el. laišką į SharePoint grupę gali nepavykti dėl "prieiga uždrausta" klaidos pranešimas, jei narystė SharePoint grupės nėra nustatyta visiems.</span><span class="sxs-lookup"><span data-stu-id="7c1a7-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="7c1a7-104">**Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:**</span><span class="sxs-lookup"><span data-stu-id="7c1a7-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="7c1a7-105">Leiskite visiems matyti SharePoint grupės narius.</span><span class="sxs-lookup"><span data-stu-id="7c1a7-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="7c1a7-106">Pašalinkite SharePoint grupę iš el. laiško eilutės Kam arba CC.</span><span class="sxs-lookup"><span data-stu-id="7c1a7-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="7c1a7-107">Aiškiai įtraukti vartotojus į eilutę kam arba CC jei narystės matomumo negalima pakeisti SharePoint grupės.</span><span class="sxs-lookup"><span data-stu-id="7c1a7-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="7c1a7-108">Norėdami peržiūrėti daugiau informacijos, prašome kreiptis į [http neleistina/_vti_bin/Client.svc/sp.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7c1a7-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  