---
title: Perdavimas el. paštu per „Microsoft 365“
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117991"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="3e159-102">Daugiafunkcio įrenginio arba programos, skirtos siųsti el. laiškus, nustatymas</span><span class="sxs-lookup"><span data-stu-id="3e159-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="3e159-103">Jei norite sužinoti apie galimas parinktis ir veiksmus, žr. [Kaip nustatyti daugiafunkcį įrenginį arba programą siųsti el. laiškus naudojant „Microsoft 365“](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="3e159-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="3e159-104">Jei turite įrenginį arba taikomąją programą, kuri neseniai nustojo veikti, dažniausiai pasitaiko problemų:</span><span class="sxs-lookup"><span data-stu-id="3e159-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="3e159-105">**Autentifikavimo susijusios klaidos naudojant SMTP autentifikavimo kliento pateikimą** Neseniai atlikome keletą pakeitimų, susijusių su SMTP autentifikavimo darbu.</span><span class="sxs-lookup"><span data-stu-id="3e159-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="3e159-106">Daugiau informacijos apie tai, kaip išspręsti problemas, žr. nesėkmingo autentifikavimo skyrių Spausdintuvų, skaitytuvų ir LOB programų, kurios siunčia [el. laiškus naudodami "Microsoft 365" arba "Office 365".](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="3e159-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="3e159-107">**Mes priimame tik TLS 1.2 versiją, kai užtikriname saugų ryšį su Office 365** Jei naudojate saugų ryšį (TLS), įsitikinkite, kad jūsų taikomosios programos įrenginys palaiko TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="3e159-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="3e159-108">Daugiau informacijos žr. [Pasirengimas TLS 1.2 Office 365 ir Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="3e159-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="3e159-109">Kitų problemų ir sprendimų ieškokite Spausdintuvų, skaitytuvų ir LOB programų, kurios siunčia el. laiškus naudodami ["Microsoft 365" arba "Office 365", problemų sprendimas.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="3e159-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="3e159-110">Norėdami peržiūrėti susijusius įrenginius, eikite į [SMTP autentifikavimo klientų ataskaitą](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3e159-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="3e159-111">**Pastaba:** Exchange Online nėra masinio pašto scenarijų.</span><span class="sxs-lookup"><span data-stu-id="3e159-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="3e159-112">Norėdami siųsti masinius komercinius el. laiškus (pvz., klientų informacinius biuletenius), turėtumėte naudoti trečiųjų šalių teikėjus, kurie specializuojasi šiose paslaugose.</span><span class="sxs-lookup"><span data-stu-id="3e159-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
