---
title: Užstrigo tarnybos importavimo užduoties trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125486"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="7eaab-102">Užstrigo tarnybos importavimo užduoties trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="7eaab-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="7eaab-103">Jei kyla problemų dėl tarnybos užduočių importavimo įstrigo arba nepavyksta, išbandykite ir bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7eaab-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="7eaab-104">Peržiūrėkite PST failo dydį.</span><span class="sxs-lookup"><span data-stu-id="7eaab-104">Review the size of of the PST file.</span></span> <span data-ttu-id="7eaab-105">Maksimalus rekomenduojamas IMPORTUOTI PST failo dydis yra 20 GB.</span><span class="sxs-lookup"><span data-stu-id="7eaab-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="7eaab-106">Jei įtariate, kad dėl sugadinimo praleisti elementai, paleiskite Scanpst.exe ir pataisykite PST failų klaidas.</span><span class="sxs-lookup"><span data-stu-id="7eaab-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="7eaab-107">Jei importavimo metu matote klaidą "MapiExceptionShutoffQuotaExceeded", įsitikinkite, kad paskirties pašto dėžutė turi pakankamai pajėgumo importuoti norimus PST failus.</span><span class="sxs-lookup"><span data-stu-id="7eaab-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="7eaab-108">Daugiau informacijos apie PST importavimo užduočių trikčių diagnostiką [žr. PST importavimo užduočių trikčių šalinimas.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="7eaab-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="7eaab-109">Informacijos, kaip išspręsti problemas importuojant PSTs į "Outlook", žr. [".pst" failo importavimo Outlook ("microsoft.com")](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="7eaab-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>