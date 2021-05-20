---
title: 2491 '테넌트 또는 사용자 오버라이드로 인해 피싱 배달' 정책에서 전자 메일 메시지 경고
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544584"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>'테넌트 또는 사용자 정의로 인해 배달된 피싱' 정책에서 전자 메일 메시지 경고

"테넌트 또는 사용자 정의로 인해 배달된 피싱"이라는 기본 경고 정책이 Microsoft Defender for Office 365 P1 및 P2 라이선스가 있는 테넌트에 롤아웃됩니다. 이 경고를 받은 경우 조사하는 단계는 다음과 같습니다.

1. 경고 메시지에서 경고  보기를 클릭하여  보안 및 준수 센터의 경고 & 이동합니다.

2. 경고를 선택하여 메시지 목록  보기 또는 탐색기에서 메시지 **보기 옵션을 볼 수 있습니다.** 이 두 옵션 모두 메시지 ID를 포함하는 메시지의 세부 정보를 제공합니다. 위협 탐색기 링크는 경고 조건과 일치하는 메시지를 자동으로 필터링합니다. 위협 탐색기에서 날짜 필터를 조정해야 할 수 있습니다.

피싱 메시지는 수동으로 구성된 다시 설정 때문에 배달됩니다.

- 사용자가 설정한 허용된 보낸 사람 또는 도메인입니다.

- 스팸 방지 정책에서 관리자가 설정한 허용된 보낸 사람 또는 도메인입니다.

- 연결 필터 정책의 허용된 IP 주소입니다.

- 메시지를 허용하도록 구성된 메일 흐름 규칙(전송 규칙)입니다.

메시지가 피싱으로 잘못 표시되었다고 생각되는 경우 보고서 [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) 메시지 Outlook 추가 기능을 사용하여 Microsoft에 메시지 샘플을 제출합니다.
