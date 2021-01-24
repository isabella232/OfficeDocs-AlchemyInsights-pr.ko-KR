---
title: 사용자 프로비저닝 특성 매핑
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935366"
---
# <a name="user-provisioning-attribute-mapping"></a>사용자 프로비저닝 특성 매핑

1. 알려진 특성 매핑 문제를 해결하려면 [특성 매핑](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)을 참조하세요. 
2. Microsoft Azure Active Directory(AD)는 Salesforce, G Suite 등의 타사 SaaS 응용 프로그램에 사용자 프로비저닝에 대한 지원을 제공합니다. 타사 SaaS 응용 프로그램에 대해 사용자 프로비저닝을 사용하도록 설정하면 Azure Portal은 특성 매핑을 통해 특성 값을 제어합니다. 기본 특성 매핑을 사용자 지정하는 방법에 대한 자세한 내용은 [Azure Active Directory에서 SaaS 응용 프로그램에 대한 사용자 프로비저닝 특성 매핑 사용자 지정](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)을 참조하세요.
    - SaaS 앱 사용자 프로비저닝에 대한 자세한 내용은 [Azure AD에서 자동화된 SaaS 앱 사용자 프로비저닝은 무엇인가요?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)를 참조하세요. 
3. 사용자 프로비저닝에 대한 특성 매핑을 사용자 지정하는 경우 매핑하려는 특성이 원본 특성 목록에 나타나지 않을 수 있습니다. [응용 프로그램 프로비저닝을 위해 온-프레미스 Active Directory에서 Azure AD로 특성 동기화](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) 문서에서는 누락된 특성을 온-프레미스 AD에서 Azure AD로 동기화하여 추가하는 방법을 설명합니다.
