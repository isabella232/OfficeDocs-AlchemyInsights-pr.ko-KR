---
title: MIM 동기화 서비스 구성
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430740"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="89da0-102">MIM 동기화 서비스 구성</span><span class="sxs-lookup"><span data-stu-id="89da0-102">Configure MIM Sync service</span></span>

<span data-ttu-id="89da0-103">Microsoft Identity Manager(MIM) 동기화 서비스는 MIM의 구성 요소입니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="89da0-104">이 서비스는 여러 개의 온-프레미스 디렉터리 및 데이터베이스가 있는 조직의 정보를 저장하고 통합하는 중앙 집중식 온-프레미스 서비스입니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="89da0-105">MIM 최신 업데이트에서 다루어졌거나 아래 섹션에 언급된 다른 문제 중 하나인 MIM 동기화 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="89da0-106">**다음 권장 단계**</span><span class="sxs-lookup"><span data-stu-id="89da0-106">**Recommended steps**</span></span>

1. <span data-ttu-id="89da0-107">MIM 동기화의 최신 업데이트를 사용하고 있는지 확인하고 [MIM 동기화 릴리스 정보](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)를 확인하여 업데이트에서 문제가 해결되었는지 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="89da0-108">일반 LDAP, 일반 SQL, Lotus Domino 또는 웹 서비스 커넥터에 문제가 있는 경우 [일반 커넥터](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)의 최신 업데이트를 사용하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="89da0-109">오류로 인해 MIM 동기화 실행이 중지되는 경우 [실행 오류 코드](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) 표를 참조하여 가능한 원인을 파악합니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="89da0-110">**extension-dll 예외** 로 실행이 중지된 경우라면 해당 단어를 클릭하여 **커넥터 공간 개체 속성** 창을 열고 **스택 추적...** 을 클릭하여 [Extension-DLL 예외](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)에 기술된 자세한 근본 원인 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="89da0-111">PCNS(암호 변경 알림 서비스) 구성 요소가 암호 동기화 동안 이벤트 로그에 **오류 6025** 를 보고하는 경우, [PCNS 보고 오류 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)를 해결하는 가이드를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="89da0-112">FIM 서비스 관리 에이전트와의 전체 동기화가 느린 경우 TempDB의 **자동 키우기** 설정을 [전체 동기화가 느리거나 중단된 경우 문제 해결](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)에 기술된 대로 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="89da0-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="89da0-113">FIM 서비스 관리 에이전트를 사용하여 웹 서비스를 통한 만들기 실패로 중지된 서버 오류가 발생하는 경우 [지원 정보: 웹 서비스를 통한 만들기 실패](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services)의 원인 개요를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="89da0-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

