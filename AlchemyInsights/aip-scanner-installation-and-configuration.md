---
title: 'AIP 스캐너: 설치 및 구성'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821669"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP 스캐너: 설치 및 구성

**AIP 스캐너를 설치하려면 다음 권장 지침을 따릅니다.**

1. 새로 설치 대신 업그레이드를 하는 경우, [Azure Information Protection 스캐너 업그레이드](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) 지침을 따르고, 통합 레이블 클라이언트의 경우, [Azure Information Protection 스캐너 업그레이드](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)를 참조하세요.
2. 전체 [방화벽 및 네트워크 인프라 설정 요구 사항](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)을 준수하는지 확인합니다.
3. 자동 레이블에 맞게 [정책이 설정되었거나](https://docs.microsoft.com/azure/information-protection/configure-policy) 정책에 기본 레이블이 설정되었는지 확인합니다.
4. [Azure Information Protection 클라이언트가 지원하는 파일 형식](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)에 설명된 대로 관련 파일 형식이 레이블/보호를 위해 구성되어 있는지 확인합니다. 또한, 기본 동작을 변경하고자 할 경우, 다음과 같은 지침을 따르세요. [파일의 기본 보호 수준 변경](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. 스캐너 서비스를 실행하도록 구성된 사용자 계정에 모든 구성 리포지토리를 액세스할 수 있는 권한이 있는지 확인합니다.
6. 문제가 계속 발생하는 경우 스캐너 로그를 내보내서 지원 티켓에 추가하세요.

**Azure Information Protection 스캐너 로그 내보내기**

1. 스캐너 서비스를 실행하는 사용자 컨텍스트 아래 %localappdata%\Microsoft\MSIP를 탐색합니다.
2. MSIP 폴더 아래에 모든 콘텐츠를 압축합니다.
3. 원하는 위치에 로그를 저장하고 서비스 요청에 첨부합니다.
4. [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)를 사용할 수도 있습니다.

**자세한 내용은 다음을 참조하세요**.
- [파일을 자동으로 분류하고 보호하는 Azure Information Protection 스캐너 배포](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication에 토큰 매개 변수 지정 및 사용](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [검색 주기 실행 및 스캐너용 보고서 보기](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Information Protection 설명서 검토](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection 요구 사항](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection 클라이언트 다운로드](https://www.microsoft.com/download/details.aspx?id=53018)
