---
title: 다양한 포트 액세스 문제에 대한 진단
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897875"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="0d377-102">다양한 포트 액세스 문제에 대한 진단</span><span class="sxs-lookup"><span data-stu-id="0d377-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="0d377-103">다양한 포트 액세스 문제를 해결하려면 다음 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="0d377-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="0d377-104">포털에서 가상 시스템(VM)을 중지/할당 취소하고 VM을 다시 시작한 후 다시 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="0d377-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="0d377-105">VM의 네트워크 설정을 확인하여 트래픽을 차단하는 NSG(네트워크 보안 그룹)가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0d377-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="0d377-106">[NetworkWatcher의 IP 흐름 확인 도구](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)를 사용하여 트래픽을 차단하는 NSG, UDR(사용자 정의 경로)을 검사하거나 트래픽을 사내('기본 경로' 0.0.0.0/0) 또는 네트워크 어플라이언스로 다시 라우팅하는지 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0d377-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="0d377-107">위의 단계를 시도한 후에도 여전히 문제가 발생하는 경우 추가 진단을 위해 메일을 보내려는 TCP 포트와 VM 이름을 제공하세요.</span><span class="sxs-lookup"><span data-stu-id="0d377-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="0d377-108">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="0d377-108">**Recommended Documents**</span></span>

[<span data-ttu-id="0d377-109">포트 25를 통해 아웃바운드 전자 메일을 보내기 위한 제한 및 권장 사항</span><span class="sxs-lookup"><span data-stu-id="0d377-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)