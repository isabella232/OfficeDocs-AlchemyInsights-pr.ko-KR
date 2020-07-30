---
title: Intune에서 Windows Defender 작업
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434597"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="76dcd-102">Intune에서 Windows Defender 작업</span><span class="sxs-lookup"><span data-stu-id="76dcd-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="76dcd-103">Intune을 사용하여 개별 장치에서 Windows Defender에 대한 요청 기반 검색 및 바이러스 서명 업데이트를 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="76dcd-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="76dcd-104">원격 작업이 트리거된 후에는 작업이 Windows Defender 이벤트 로그에 반영됩니다.</span><span class="sxs-lookup"><span data-stu-id="76dcd-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="76dcd-105">Windows Endpoint Protection 정책을 사용하면 Intune에서 Windows Defender 기능의 추가 설정을 만들고 장치 집합에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="76dcd-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="76dcd-106">Windows Defender 작업을 트리거하는 방법에 대한 자세한 내용은 [Microsoft Defender 바이러스 백신 검색 구성 및 실행](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="76dcd-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>