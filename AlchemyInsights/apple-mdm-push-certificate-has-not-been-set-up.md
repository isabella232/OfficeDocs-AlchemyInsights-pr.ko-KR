---
title: Apple MDM Push 인증서가 설정되지 않음
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
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716863"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push 인증서가 설정되지 않음

Apple MDM Push 인증서(APNS(Apple Push Notification Service))가 사용자 구독에 구성되지 않았습니다. Apple MDM Push 인증서가 구성되지 않으면 iOS 및 MacOS 장치를 등록하고 관리할 수 없습니다. Intune에 인증서를 추가한 후 사용자가 회사 포털 앱을 설치하여 iOS 장치를 등록할 수 있습니다.

1. **"동의"** 를 선택합니다. Microsoft가 Apple에 데이터를 보낼 수 있는 권한을 부여합니다.

2. Apple MDM Push 인증서를 만드는 데 필요한 Intune 인증서 서명 요청 **CSR 다운로드**를 선택합니다. Apple Push 인증서 포털에서 신뢰 관계 인증서를 요청하려면 이 파일이 필요합니다.

3. **MDM Push 인증서 만들기**를 선택하여 Apple Push 인증서 포털로 이동합니다. 회사 Apple ID를 사용하여 로그인 한 다음 **인증서 만들기**를 선택합니다. **파일 선택** 선택하고 인증서 서명 요청 파일을 찾은 다음 **업로드**를 선택합니다. 확인 페이지에서 **다운로드**를 선택하여 인증서(.pem) 파일을 다운로드 하고 로컬에 파일을 저장합니다.
 
**참고**: 인증서는 이를 만드는 데 사용 되는 Apple ID와 관련 있습니다. 모범 사례는 관리 업무에 회사 Apple ID로 한 명 이상의 사람이나 배포 목록을 사용하여 사서함이 모니터링 되는지 확인하는 것입니다. 개인 Apple ID를 사용해 서는 안 됩니다. 동일 Apple ID를 사용하여 12개월 마다 Apple Push 인증서를 갱신합니다.
 
4. Apple MDM Push 인증서를 만드는데 사용한 Apple ID를 입력합니다. 인증서를 갱신해야 하는 경우를 대비해 이 ID를 미리 알림으로 기록합니다.

5. 인증서 (pem) 파일로 이동하고 **열기**를 선택한 다음 **업로드**를 선택합니다. Push 인증서를 사용하여 Intune에서 Apple 장치를 등록하고 관리할 수 있습니다.