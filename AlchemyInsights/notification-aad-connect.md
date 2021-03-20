---
title: 알림 AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898043"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="654a0-102">알림 AAD Connect</span><span class="sxs-lookup"><span data-stu-id="654a0-102">Notification AAD Connect</span></span>

- <span data-ttu-id="654a0-103">작업을 수행할 수 있는 권한이 부여된지 확인</span><span class="sxs-lookup"><span data-stu-id="654a0-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="654a0-104">전역 관리자는 기본적으로 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="654a0-104">Global Admins have access by default.</span></span> <span data-ttu-id="654a0-105">또한 역할 기반 액세스 [제어를](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 사용하여 참가자에게 등록 권한을 위임할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="654a0-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="654a0-106">필요한 끝점이 사용하도록 설정되어 있으며 방화벽으로 인해 차단되지 않는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="654a0-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="654a0-107">자세한 내용은 요구 사항을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="654a0-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="654a0-108">네트워크 계층에 의해 SSL 검사가 진행되는 아웃바운드 통신으로 인해 등록이 실패할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="654a0-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="654a0-109">Azure AD Connect Health에 대한 알림 설정을 확인한 후 설정을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="654a0-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="654a0-110">Azure AD Connect Health 알림에 대한 알림 설정을 구성하는 방법을 이해하려면 이 가이드를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="654a0-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="654a0-111">AAD Connect 상태 동기화 보고서 및 다운로드 방법에 대한 자세한 내용은 개체 수준 동기화 [보고서 를 참조합니다.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="654a0-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="654a0-112">AAD Connect 상태 경고 문제를 해결하기 위해 AAD Connect Health [Data freshness Alerts에](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 대한 문제 해결 가이드와 일반적으로 묻는 질문은 [Common AAD Connect Health installation questions을 참조하십시오.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="654a0-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
