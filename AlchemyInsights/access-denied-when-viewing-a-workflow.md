---
title: Prieiga uždrausta peržiūrint darbo eigą
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688810"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="cb025-102">Prieiga uždrausta peržiūrint darbo eigą</span><span class="sxs-lookup"><span data-stu-id="cb025-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="cb025-103">Jei "SharePoint" grupės narystė nenustatyta visiems, "SharePoint" 2013 darbo eigos, kurios bando siųsti laišką "SharePoint" grupei, gali nepavykti naudojant klaidos pranešimą "prieiga uždrausta".</span><span class="sxs-lookup"><span data-stu-id="cb025-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="cb025-104">**Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:**</span><span class="sxs-lookup"><span data-stu-id="cb025-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="cb025-105">Leiskite visiems matyti "SharePoint" grupės narius.</span><span class="sxs-lookup"><span data-stu-id="cb025-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="cb025-106">Pašalinkite "SharePoint" grupę iš el. laiško eilutės Kam arba kopija.</span><span class="sxs-lookup"><span data-stu-id="cb025-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="cb025-107">Tiesiogiai įtraukti vartotojus į eilutę kam arba kopija, jei "SharePoint" grupėje negalima pakeisti narystės matomumo.</span><span class="sxs-lookup"><span data-stu-id="cb025-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="cb025-108">Norėdami peržiūrėti daugiau informacijos, žr [http neleistinas/_vti_bin/Client.svc/sp.utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="cb025-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  