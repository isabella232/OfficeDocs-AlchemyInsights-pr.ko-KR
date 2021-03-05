---
title: 네트워크 검사 사용 안
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449105"
---
# <a name="disable-network-scan"></a><span data-ttu-id="4a1c5-102">네트워크 검사 사용 안</span><span class="sxs-lookup"><span data-stu-id="4a1c5-102">Disable network scan</span></span>

<span data-ttu-id="4a1c5-103">네트워크 공유 검사는 성능에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4a1c5-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="4a1c5-104">클라이언트가 기본적으로 네트워크 공유/파일을 검색하지 않도록 설정하려면 Windows Defender 응용 프로그램에서 다음 설정을 **True로 구성합니다.**</span><span class="sxs-lookup"><span data-stu-id="4a1c5-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="4a1c5-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="4a1c5-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="4a1c5-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="4a1c5-106">DisableScanningNetworkFiles</span></span>