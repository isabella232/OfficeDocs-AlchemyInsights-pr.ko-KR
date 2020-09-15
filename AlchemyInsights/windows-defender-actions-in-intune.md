---
title: Intune에서 Windows Defender 작업
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 732b7450121f85416bb0f1868b3722899bee8194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699093"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="d8e21-102">Intune에서 Windows Defender 작업</span><span class="sxs-lookup"><span data-stu-id="d8e21-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="d8e21-103">Intune을 사용하여 개별 장치에서 Windows Defender에 대한 요청 기반 검색 및 바이러스 서명 업데이트를 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d8e21-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="d8e21-104">원격 작업이 트리거된 후에는 작업이 Windows Defender 이벤트 로그에 반영됩니다.</span><span class="sxs-lookup"><span data-stu-id="d8e21-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="d8e21-105">Windows Endpoint Protection 정책을 사용하면 Intune에서 Windows Defender 기능의 추가 설정을 만들고 장치 집합에 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d8e21-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="d8e21-106">Windows Defender 작업을 트리거하는 방법에 대한 자세한 내용은 [Microsoft Defender 바이러스 백신 검색 구성 및 실행](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d8e21-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>