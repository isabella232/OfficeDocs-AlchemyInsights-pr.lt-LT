---
title: PPK žymių strategijų kūrimo
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732183"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a7ad5-102">PPK žymių strategijų kūrimo</span><span class="sxs-lookup"><span data-stu-id="a7ad5-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a7ad5-103">"Azure" informacijos apsaugos (AIP) etiketes galima naudoti su visu duomenų diapazonu, kurį organizacija paprastai sukuria ir saugo pagal mažiausią asmens duomenų klasifikaciją pagal aukščiausią labai konfidencialių duomenų klasifikaciją.</span><span class="sxs-lookup"><span data-stu-id="a7ad5-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a7ad5-104">"Azure" informacijos apsaugos strategijos taikomos "Azure" informacijos apsaugos (AIP) klasikiniam klientui, o ne "  [aip](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)".</span><span class="sxs-lookup"><span data-stu-id="a7ad5-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a7ad5-105">Galite konfigūruoti kelis elementus "AIP" politikoje, įskaitant tokias parinktis:</span><span class="sxs-lookup"><span data-stu-id="a7ad5-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a7ad5-106">Parinktis, kurios žymė leis administratoriams arba vartotojams klasifikuoti ir apsaugoti (pasirinktinai) dokumentus ir elektroninius laiškus</span><span class="sxs-lookup"><span data-stu-id="a7ad5-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a7ad5-107">Galimybė vykdyti klasifikavimą, kai vartotojai įrašo dokumentus ir siunčia laišką</span><span class="sxs-lookup"><span data-stu-id="a7ad5-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a7ad5-108">Parinktis automatiškai žymėti el. laišką, atsižvelgiant į jo priedus.</span><span class="sxs-lookup"><span data-stu-id="a7ad5-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a7ad5-109">Parinktis valdyti, ar "Office" taikomosiose programose rodoma informacijos apsaugos juosta</span><span class="sxs-lookup"><span data-stu-id="a7ad5-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a7ad5-110">Jei turite papildomų parinkčių ir informacijos apie "Azure" informacijos apsaugos strategijas, žiūrėkite: " [Azure" informacijos apsaugos strategijos apžvalga](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a7ad5-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a7ad5-111">Kitų naudingų išteklių, susijusių su Ail strategijomis, ieškokite:</span><span class="sxs-lookup"><span data-stu-id="a7ad5-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a7ad5-112">Vadovėlis: "Azure" informacijos apsaugos strategijos parametrų konfigūravimas ir naujos Žymos kūrimas</span><span class="sxs-lookup"><span data-stu-id="a7ad5-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a7ad5-113">"Azure" informacijos apsaugos strategijos konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="a7ad5-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a7ad5-114">Jautrumo žymių ir jų strategijų kūrimas ir konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="a7ad5-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a7ad5-115">Bendrųjų scenarijų, kurie naudoja "Azure" informacijos apsaugą, vadovai</span><span class="sxs-lookup"><span data-stu-id="a7ad5-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a7ad5-116">"Azure" informacijos apsaugos dokumentų peržiūra</span><span class="sxs-lookup"><span data-stu-id="a7ad5-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a7ad5-117">"Azure" informacijos apsaugos reikalavimai</span><span class="sxs-lookup"><span data-stu-id="a7ad5-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a7ad5-118">"Azure" informacijos apsaugos greito pasirengimo darbui vadovas</span><span class="sxs-lookup"><span data-stu-id="a7ad5-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a7ad5-119">Atsisiųsti "Azure" informacijos apsaugos klientą</span><span class="sxs-lookup"><span data-stu-id="a7ad5-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)