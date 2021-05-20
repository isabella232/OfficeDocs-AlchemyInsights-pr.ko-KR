---
title: Microsoft Defender ATP 검색에 대한 예외 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543691"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="7c541-102">Microsoft Defender ATP 검색에 대한 예외 구성</span><span class="sxs-lookup"><span data-stu-id="7c541-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="7c541-103">일반적으로 Microsoft Defender ATP 검색에서 특정 파일 확장명 및 폴더 위치를 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7c541-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="7c541-104">또한 특정 프로세스에서 연 파일에 대한 제외 항목을 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7c541-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="7c541-105">자세한 내용은 [파일 확장명 및 폴더 위치를 기준으로 제외 구성 및 확인](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) 및 [프로세스에서 연 파일에 대한 제외 구성](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="7c541-106">**Windows Server 2016 및 2019** 에 대한 제외 항목을 구성하려면 [Windows Server에서Microsoft Defender 바이러스 백신 제외 구성](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="7c541-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="7c541-107">**Mac**</span></span>

<span data-ttu-id="7c541-108">지원되는 제외 유형 및 Mac용 제외 목록 구성에 대한 자세한 내용은 [지원되는 제외 유형](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) 및 [제외 목록을 구성하는 방법](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="7c541-109">**참고** EICAR 테스트 파일을 사용하여 제외 목록을 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7c541-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="7c541-110">자세한 내용은 [EICAR 테스트 파일을 사용하여 제외 목록 확인](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="7c541-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="7c541-111">**Linux**</span></span>

<span data-ttu-id="7c541-112">지원되는 제외 유형 및 Linux에 대한 제외 목록 구성에 대한 자세한 내용은 [지원되는 제외 유형](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) 및 [Linux용 Microsoft Defender ATP에 대한 제외 구성 및 유효성 검사](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="7c541-113">**참고** EICAR 테스트 파일을 사용하여 제외 목록을 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7c541-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="7c541-114">자세한 내용은 [EICAR 테스트 파일을 사용하여 제외 목록 확인](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7c541-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 