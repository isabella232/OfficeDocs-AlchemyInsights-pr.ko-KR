---
title: 메일 그룹에 외부 사용자 추가
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663519"
---
# <a name="add-external-users-to-a-distribution-group"></a>메일 그룹에 외부 사용자 추가

DG (메일 그룹)에 외부 연락처를 추가 하는 과정은 두 단계로 진행 됩니다.
  
1. 외부 사용자에 대 한 메일 연락처를 만듭니다.
    
    1. 관리 센터에서 **사용자**  >  [연락처](https://admin.microsoft.com/adminportal/home#/Contact) 페이지로 이동 합니다. 
    
    2. **연락처 추가를**선택 합니다.
    
    3. 연락처에 대 한 정보를 입력 하 고 **추가**를 선택 합니다.
    
2. DG에 메일 연락처를 추가 합니다.
    
    1. 관리 센터에서 **그룹**  >  [그룹](https://admin.microsoft.com/adminportal/home#/groups) 페이지로 이동 합니다. 
    
    2. 외부 사용자를 추가할 DG를 찾아서 선택 하 여 편집 대화 상자를 엽니다.
    
    3. **구성원** 탭에서 **모두 보기 및 구성원 관리**를 선택 합니다. 
    
    4. **구성원 추가**를 선택합니다.
    
    5. 이전 단계에서 만든 메일 연락처를 선택한 다음 **저장**을 선택 합니다.
    
이러한 단계를 수행한 후에 외부 사용자가 DG로 전자 메일을 보내거나 보내지 못하는 경우에는 내부 사용자의 전자 메일만 허용 하도록 DG가 표시 될 수 있습니다. 이 구성을 확인 하 고 [여기에 나와](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)있는 지침을 따라 문제를 해결할 수 있습니다.
  
 **참고:** 그룹 유형이 "메일 그룹" 대신 "Microsoft 365 group" 인 경우에는 이러한 지침이 적용 되지 않습니다. 이 경우 외부 사용자를 Outlook에서 그룹에 직접 추가할 수 있습니다. [이 문서](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)에서는 Microsoft 365 그룹 게스트와 외부 게스트를 추가 하는 방법에 대 한 자세한 정보를 확인할 수 있습니다.
  