---
title: Ankstesnių "Office" MSI versijų šalinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680726"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="61173-102">Ankstesnių "Office" MSI versijų šalinimas</span><span class="sxs-lookup"><span data-stu-id="61173-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="61173-103">Rekomenduojame pašalinti ankstesnes "Windows Installer" (MSI) "Office" versijas prieš diegiant "Office 365 ProPlus".</span><span class="sxs-lookup"><span data-stu-id="61173-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="61173-104">Štai kaip tai padaryti:</span><span class="sxs-lookup"><span data-stu-id="61173-104">Here's how to do this:</span></span>

1. <span data-ttu-id="61173-105">Jei naudojote MSI, kad įdiegtumėte "Office", galite naudoti "Office" diegimo įrankį (ODT), kad pašalintumėte "Office".</span><span class="sxs-lookup"><span data-stu-id="61173-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="61173-106">Galite naudoti "RemoveMSI" elementą **configuration.xml** faile.</span><span class="sxs-lookup"><span data-stu-id="61173-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="61173-107">Vadovaukitės šiame straipsnyje pateikiamais nurodymais: " [Office 365" saugos & atitikties centras.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="61173-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>