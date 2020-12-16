---
title: 전송 서비스 - 모든 RDFE 서비스를 다른 구독으로 이동
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681478"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>전송 서비스 - 모든 RDFE 서비스를 다른 구독으로 이동

**자원 이동**

Azure Portal, Azure PowerShell, Azure CLI 또는 REST API를 사용하여 동일한 구독의 다른 Azure 구독 또는 리소스 그룹으로 Azure 리소스를 이동할 수 있습니다.

리소스를 이동하기 전에 다음을 참조합니다.

- [자원 이동 전 검사 목록](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [이동할 수 있는 서비스](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [이동의 유효성을 검사하는 방법](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [서비스에 대한 이동 지침](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

기존 리소스를 다른 리소스 그룹 또는 구독으로 이동하려면 다음을 사용할 수 있습니다.

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

자습서: Azure 리소스를 다른 리소스 그룹 또는 [구독으로 이동](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resource Manager를 사용하여 오류 해결**

아래의 문서를 참조하여 몇 가지 일반적인 Azure 배포 오류에 대해 알아보고 문제를 해결하기 위한 정보를 받으세요. 배포 오류에 대한 오류 코드를 찾을 수 없는 경우 오류 [코드 찾기를 참조합니다.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [배포 오류 해결](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure 리소스를 새 리소스 그룹 또는 구독으로 이동하는 문제 해결](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

무료에서 유료로 전환하는 등 Azure 구독을 업그레이드하려면 구독을 변환해야 합니다.

- 무료 평가판을 업그레이드하려면 무료 평가판 업그레이드 또는 Microsoft Azure 구독을 유료로 업그레이드를 [참조하세요.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- 유료 계정을 변경하려면 [Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)구독을 다른 제품으로 변경하세요.

**Azure 구독을 추가하거나 Azure Active Directory 테넌트에 연결하려면**

1. 로그인하고 Azure Portal의 구독 페이지에서 사용할 [구독을 선택합니다.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. 디렉터리 **변경을 선택합니다.**
3. 나타나는 경고를 검토한 다음 변경을 **선택합니다.**
4. 구독에 대한 디렉터리가 변경된 경우 성공 메시지가 표시됩니다.
5. 디렉터리 *전환을* 사용하여 새 디렉터리로 이동하십시오. 모든 것이 제대로 표시될 때 최대 10분이 걸릴 수 있습니다.

**권장 문서**

- [Azure 구독 소유권 이전](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [자원을 새 리소스 그룹 또는 구독으로 이동](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Azure Portal을 사용하여 리소스 관리](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
