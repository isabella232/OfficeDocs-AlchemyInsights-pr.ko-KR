---
title: 온-프레미스 서버에서 분리 된 사용자 삭제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680141"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>온-프레미스 서버에서 분리 된 사용자 삭제

분리 된 사용자를 삭제하려면 다음 단계를 따릅니다.

1. [Azure Active Directory에서 하이브리드 ID가 무엇인가요?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)의 지침에 따라 디렉토리 동기화를 강제로 수행합니다.

2. 디렉토리 동기화를 확인하려면 [Azure Active Directory에서 하이브리드 ID가 무엇인가요?](https://technet.microsoft.com/library/jj151797.aspx)를 참조하세요.

3. 동기화 기능이 제대로 작동하지 않지만 활성 디렉토리 객체 삭제가 Azure AD에 전파되지 않는 경우 다음 Windows PowerShell cmdlets용 Azure Active Directory 모듈 중 하나를 사용하여 분리된 개체를 수동으로 제거하세요.

    제거-MsolContact  
    제거-MsolGroup  
    제거-MsolUser

    예를 들어, 디렉토리 동기화를 사용하여 만들어진 분리된 사용자 ID john.smith@contoso.com를 제거하려면 cmdlet을 실행합니다.

    제거-MsolUser –UserPrincipalName John.Smith@Contoso.com