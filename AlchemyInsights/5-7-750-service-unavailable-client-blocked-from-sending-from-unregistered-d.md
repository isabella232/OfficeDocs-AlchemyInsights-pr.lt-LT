---
title: 1048 5.7.750 Tarnyba nepasiekiama. Klientas užblokavo siuntimą iš neregistruotų domenų
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774259"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="82767-103">5.7.750 Klientas užblokuotas siųsti iš neregistruoto domeno</span><span class="sxs-lookup"><span data-stu-id="82767-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="82767-104">Klaida įvyksta, kai didelis pranešimų kiekis siunčiamas iš domenų, kurie nėra parengti jūsų nuomotojui (įtraukta kaip pripažinti domenai ir patikrinta).</span><span class="sxs-lookup"><span data-stu-id="82767-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="82767-105">Norėdami išvengti šios klaidos, galite naudoti sertifikatu pagrįstą pašto srauto jungtį, kurioje sertifikato domenas yra parengimo domenas, arba galite parengti visus siuntimo domenus.</span><span class="sxs-lookup"><span data-stu-id="82767-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="82767-106">Daugiau informacijos žr. El. pašto pristatymo problemų sprendimas, kai klaidų kodai [yra nuo 5.7.700 iki 5.7.750 Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="82767-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>