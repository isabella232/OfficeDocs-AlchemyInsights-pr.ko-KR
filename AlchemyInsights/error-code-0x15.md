---
title: 오류 코드 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: RDS (원격 데스크톱 서비스) 배포에서 Office 2013을 정품 인증 하는 동안 오류가 발생 하는 경우 레지스트리를 편집 하 여 ADAL을 사용 하도록 설정 하는 것이 좋습니다.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506852"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>원격 데스크톱 서비스에서 Office 2013 정품 인증을 진행 하는 동안 오류 발생

RDS (원격 데스크톱 서비스) 배포에서 Office 2013을 정품 인증 하는 동안 오류가 발생 하는 경우 레지스트리를 편집 하 여 ADAL을 사용 하도록 설정 하는 것이 좋습니다.
  
|**레지스트리 키**|**유형**|**값**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

자세한 내용은 [Windows 장치에서 Office 2013에 대 한 최신 인증 사용](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)을 참조 하세요.
  
> [!NOTE]
>  Microsoft 365 Apps for enterprise 및 Office 2016에서는 ADAL이 기본적으로 사용 하도록 설정 되어 있습니다. 이전에는 RDS (원격 데스크톱 서비스)를 터미널 서비스 라고 합니다.
  