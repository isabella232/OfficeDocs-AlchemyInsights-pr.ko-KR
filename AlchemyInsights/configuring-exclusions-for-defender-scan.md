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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768487"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="9a557-102">Microsoft Defender ATP 검색에 대한 예외 구성</span><span class="sxs-lookup"><span data-stu-id="9a557-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="9a557-103">일반적으로 Microsoft Defender ATP 검색에서 특정 파일 확장명 및 폴더 위치를 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9a557-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="9a557-104">또한 특정 프로세스에서 연 파일에 대한 제외 항목을 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9a557-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="9a557-105">자세한 내용은 [파일 확장명 및 폴더 위치를 기준으로 제외 구성 및 확인](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) 및 [프로세스에서 연 파일에 대한 제외 구성](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="9a557-106">**Windows Server 2016 및 2019** 에 대한 제외 항목을 구성하려면 [Windows Server에서Microsoft Defender 바이러스 백신 제외 구성](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="9a557-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="9a557-107">**Mac**</span></span>

<span data-ttu-id="9a557-108">지원되는 제외 유형 및 Mac용 제외 목록 구성에 대한 자세한 내용은 [지원되는 제외 유형](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) 및 [제외 목록을 구성하는 방법](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="9a557-109">**참고** EICAR 테스트 파일을 사용하여 제외 목록을 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9a557-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9a557-110">자세한 내용은 [EICAR 테스트 파일을 사용하여 제외 목록 확인](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="9a557-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="9a557-111">**Linux**</span></span>

<span data-ttu-id="9a557-112">지원되는 제외 유형 및 Linux에 대한 제외 목록 구성에 대한 자세한 내용은 [지원되는 제외 유형](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) 및 [Linux용 Microsoft Defender ATP에 대한 제외 구성 및 유효성 검사](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="9a557-113">**참고** EICAR 테스트 파일을 사용하여 제외 목록을 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9a557-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9a557-114">자세한 내용은 [EICAR 테스트 파일을 사용하여 제외 목록 확인](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9a557-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 