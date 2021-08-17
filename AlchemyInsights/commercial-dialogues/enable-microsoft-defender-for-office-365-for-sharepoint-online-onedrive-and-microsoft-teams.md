---
title: "\"Seifas\", \"SharePoint Online\", \"\"OneDrive\"\" ir \"Microsoft Teams"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894471"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>"Seifas", "SharePoint Online", ""OneDrive"" ir "Microsoft Teams

1. Naudodami savo visuotinio administratoriaus arba saugos administratoriaus kredencialus, atidarykite ""Microsoft 365" sargyba" portalą , tada eikite <https://security.microsoft.com> į Strategijos & **taisyklės** \>  \> **Grėsmių strategijos Seifas Priedai** skyriuje Strategijos 

   Norėdami pereiti tiesiai į **Seifas priedų puslapį,** naudokite <https://security.microsoft.com/safeattachmentv2> .

2. Puslapyje **Seifas priedai spustelėkite** **Visuotiniai parametrai**.
3. Rodomame iškeliame meniu pasirinkite Įjungti **"Microsoft" sargybą Office 365, SharePoint, "OneDrive" ir Microsoft Teams**, tada pasirinkite **Įrašyti**.

    > [!TIP]
    >
    > Atlikite šiuos veiksmus, kad padidintų "Seifas", "SharePoint", ""OneDrive"" ir "Microsoft Teams" apsaugą:
    >
    > - Norėdami neleisti vartotojams atsisiųsti kenkėjiškų failų, naudokite `$true` parametro *DisallowInfectedFileDownload* reikšmę "SharePoint Online PowerShell" **[set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** cmdlet. Daugiau informacijos žr. [Internetinės "PowerShell SharePoint naudojimas norint neleisti vartotojams atsisiųsti kenkėjiškų failų.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Aptiktų failų įspėjimo strategijos kūrimas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Daugiau informacijos [žr. Seifas priedų Office 365, SharePoint "OneDrive" ir Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
