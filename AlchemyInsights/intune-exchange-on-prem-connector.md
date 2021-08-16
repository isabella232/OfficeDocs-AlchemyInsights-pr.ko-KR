---
title: Intune Exchange 커넥터
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013970"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange 커넥터

Intune과 Exchange 커넥터를 설정하는 자세한 내용은 다음 설명서를 참조하십시오.

[Azure에서 Intune Exchange Microsoft Intune 커넥터 설정](https://docs.microsoft.com/intune/exchange-connector-install)

**자주 묻는 질문(FAQ):**

Q: Exchange 커넥터를 설정하려고 할 때 "Exchange 커넥터 버전이 지원되지 않습니다."라는 오류가 Exchange 있습니다. 원인은 무엇입니까?

A: 사용하는 계정이 적절하게 라이선스가 부여됩니다. 활성 Intune 라이선스가 있어야 합니다.

Q: 여러 개의 연결선이 있을 Exchange 있습니까?

A: 조직당 Intune 테넌트당 하나의 Exchange 커넥터만 설정할 Exchange 있습니다. 커넥터는 다중 서버 교환 조직의 한 서버에만 설치할 수 있습니다.

또한 동일한 테넌트에 구성한 Exchange 및 Exchange Online 커넥터를 구성할 수 없습니다.

Q: 커넥터가 CAS 배열을 CAS 배열을 연결에 사용할 수 Exchange?

A: 커넥터 설정에서 CAS 배열을 지정하는 것은 지원되지 않습니다. 단일 서버만 지정하고 에서 찾을 수 있는 커넥터 구성 파일에서 하드코드해야 합니다.

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

다음 항목을 찾아 ```<ExchangeWebServiceURL />``` URL을 Exchange 서버로 바 사용합니다.

**예제:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

추가 문제 해결에 대한 자세한 내용은 다음 설명서를 참조하십시오. [Intune의 사내](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) 커넥터 문제 Exchange 참조하세요.

**커넥터에 대해 자세한 Exchange 사용**

1. 편집할 Exchange 커넥터 추적 구성 파일을 니다.  
파일은 %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**예제:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. OnPremisesExchangeConnectorService 키를 사용하여 TraceSourceLine을 찾습니다.  
  
3. SourceLevel 노드 값을 Information ActivityTracing(기본값)에서 Verbose ActivityTracing으로 변경  

**예제:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune Exchange 서비스 다시 시작  
5. 완료될 때까지 Intune 포털에서 전체 동기화를 마친 다음 XML을 "Information ActivityTracing"으로 다시 변경하고 Microsoft Intune Exchange 서비스를 다시 시작합니다.  
6. 로그의 위치는 입니다. `%ProgramData%\Microsoft\Windows Intune Exchange Connector`