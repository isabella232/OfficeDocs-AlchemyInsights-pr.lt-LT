---
title: Importavimas ir eksportavimas iš "Yammer"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036121"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="78f72-102">Importavimas ir eksportavimas iš "Yammer"</span><span class="sxs-lookup"><span data-stu-id="78f72-102">Import and export from Yammer</span></span>

<span data-ttu-id="78f72-103">**Importuoti**</span><span class="sxs-lookup"><span data-stu-id="78f72-103">**Import**</span></span>

<span data-ttu-id="78f72-104">Vartotojo importavimo parinktys gali skirtis, atsižvelgiant į tai, ar jūsų "Yammer" tinklas yra [vietinis režimas, skirtas "Microsoft 365"](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), ar ne.</span><span class="sxs-lookup"><span data-stu-id="78f72-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="78f72-105">**Neprigimtinis režimas**: vartotojus galima importuoti į grupes naudojant " [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) " ("100" vartotojų) grupės parametruose arba tinkle naudojant [masinį naujinimą](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) tinklo administratorius.</span><span class="sxs-lookup"><span data-stu-id="78f72-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="78f72-106">**Prigimtinis režimas**: grupės narystė ir tinklo narystės operacijos turi būti atliekamos iš ["Microsoft" 365 administravimo portalo, "](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD" portalo](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)arba naudojant kitą "Azure AD" parinktį.</span><span class="sxs-lookup"><span data-stu-id="78f72-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="78f72-107">Vietiniu režimu esantys tinklai nebeturi prieigos prie masinio naujinimo ir kitų senstelėjusių funkcijų.</span><span class="sxs-lookup"><span data-stu-id="78f72-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="78f72-108">"Yammer" niekada nepalaikė turinio importavimo iš tinklo administratoriaus net tada, kai duomenų eksportavimo funkcija buvo naudota kitame tinkle.</span><span class="sxs-lookup"><span data-stu-id="78f72-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="78f72-109">Turinys gali būti iš naujo paskelbtas partnerių sprendimais arba "Yammer" kitų API.</span><span class="sxs-lookup"><span data-stu-id="78f72-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="78f72-110">**Eksportuoti**</span><span class="sxs-lookup"><span data-stu-id="78f72-110">**Export**</span></span>

<span data-ttu-id="78f72-111">[Eksportuokite tinklo duomenis tinklo administratorius](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) leidžia eksportuoti turinį iš "Yammer" tinklų, įskaitant pranešimą ir failus.</span><span class="sxs-lookup"><span data-stu-id="78f72-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="78f72-112">Priedai gali būti labai dideli ir dėl to eksportuos gali užtrukti, kol bus baigta.</span><span class="sxs-lookup"><span data-stu-id="78f72-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="78f72-113">Rekomenduojame, kad aktyvūs tinklai būtų eksportuojami naudojant [duomenų eksportavimo API](https://developer.yammer.com/docs/data-export-api) į gabaliukus pagal dieną ar savaitę.</span><span class="sxs-lookup"><span data-stu-id="78f72-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="78f72-114">"Microsoft" palaikymas neteikia šio tikslo pasirinktiniams scenarijams.</span><span class="sxs-lookup"><span data-stu-id="78f72-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="78f72-115">Atskiras [Gdpr eksportavimas](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) yra skirtas atskiro vartotojo turiniui eksportuoti.</span><span class="sxs-lookup"><span data-stu-id="78f72-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>