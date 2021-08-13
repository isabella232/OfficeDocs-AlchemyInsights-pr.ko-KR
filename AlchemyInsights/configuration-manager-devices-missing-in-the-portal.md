---
title: 포털에 누락된 Configuration Manager 장치
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
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966115"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>포털에 누락된 Configuration Manager 장치

장치 동기화가 작동하려면 서비스 연결 지점 역할을 호스팅하는 온-프레미스 서버에서 [필수 인터넷 끝점](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)을 연결할 수 있어야 합니다. 장치 동기화 문제를 해결하려면 서비스 연결 지점에 있는 **CMGatewaySyncUploadWorker.log** 를 검토하세요.

[Microsoft 끝점 관리자에서 테넌트 연결](https://docs.microsoft.com/configmgr/tenant-attach/)에 대해서 자세히 알아보세요.
