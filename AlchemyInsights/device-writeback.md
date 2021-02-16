---
title: 장치 쓰기백
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255172"
---
# <a name="device-writeback"></a><span data-ttu-id="d58e0-102">장치 쓰기백</span><span class="sxs-lookup"><span data-stu-id="d58e0-102">Device Writeback</span></span>

<span data-ttu-id="d58e0-103">장치 쓰기 기록은 다음과 같은 시나리오에서 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="d58e0-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="d58e0-104">하이브리드 인증서 신뢰 배포를 사용하여 비즈니스용 [Windows Hello 사용](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="d58e0-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="d58e0-105">ADFS(2012 R2 이상) 보호된 응용 프로그램(신뢰하는 사용자 트러스트)에 대한 장치에 기반한 조건부 액세스 사용</span><span class="sxs-lookup"><span data-stu-id="d58e0-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="d58e0-106">디바이스 쓰기 저장소를 위해 Azure AD Premium 구독이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d58e0-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="d58e0-107">이렇게 하면 응용 프로그램에 대한 액세스가 신뢰할 수 있는 디바이스에만 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="d58e0-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="d58e0-108">조건부 액세스에 대한 자세한 [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) 내용은 조건부 액세스로 위험 관리 및 Azure Active Directory 장치 등록을 사용하여 [On-premises 조건부 액세스를 설정하는 방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="d58e0-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="d58e0-109">장치에 대해 장치 쓰기 기록을 사용하도록 설정하는 데 대한 자세한 내용은 장치 쓰기 기록 [사용을 참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="d58e0-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
