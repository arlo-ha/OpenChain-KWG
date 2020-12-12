---
title: "2. 샘플 오픈소스 컴플라이언스 프로세스"
weight: 2
type: docs
---
오픈소스 컴플라이언스의 주요 두 가지 목적은 다음과 같다.

1. 라이선스 의무 파악 : 배포 대상 소프트웨어가 포함하고 있는 오픈소스를 식별하고 각 오픈소스 라이선스가 요구하는 의무를 파악한다.
2. 라이선스 의무 사항 이행 : 식별한 의무 사항을 이행한다.

이를 위해 기업은 배포 대상 소프트웨어를 배포하는 시점에 오픈소스 라이선스 의무사항을 준수할 수 있도록 오픈소스 컴플라이언스 프로세스를 구축해야 한다. 여기서는 일반적인 오픈소스 컴플라이언스 프로세스의 구성요소와 각각의 기능 및 역할을 포함하는 프로세스(예시)를 제안한다. 

{{< alert title="Note:" >}}
이 샘플 오픈소스 컴플라이언스 프로세스는 다음 자료를 참고하여 작성하였다. 

* Open Source Compliance In The Enterprise / Ibrahim Haddad : [https://www.linuxfoundation.org/compliance-and-security/2018/12/open-source-compliance-in-the-enterprise/](https://www.linuxfoundation.org/compliance-and-security/2018/12/open-source-compliance-in-the-enterprise/)

{{< /alert >}}

## 1. 오픈소스 컴플라이언스 프로세스

소프트웨어 개발 시 오픈소스를 사용하기 위해서는 기업의 오픈소스 정책에 근거하여 먼저 오픈소스 라이선스가 무엇인지 식별하고, 라이선스가 요구하는 의무 사항을 검토하고 확인해야 한다. 그리고 각 소프트웨어를 배포 시 각 오픈소스 라이선스가 요구하는 의무사항을 준수하기 위한 활동을 수행한다. 이를 오픈소스 컴플라이언스 활동이라고 한다.

기업의 오픈소스 컴플라이언스 프로세스는 배포 대상 소프트웨어에 사용되는 오픈소스를 관리하는 일련의 과정을 정의한다. 이 과정에는 다음 사항이 포함된다.

1. 배포 대상 소프트웨어에 사용된 모든 오픈소스 식별
2. 식별한 오픈소스에 의해 발생하는 모든 라이선스 의무를 식별하고 기록
3. 모든 라이선스 의무를 충족하기 위한 활동 수행

이를 효과적으로 수행하기 위해 기업의 모든 프로그램 참여자는 다음 10단계를 수행한다. 

### Step 1. 오픈소스 식별 (Identification of Open Source)

![](../step1.png)

오픈소스 식별 단계는 배포 대상 소프트웨어에 포함된 오픈소스를 식별하는 단계이다. 자체 독점 소프트웨어인지, 제3자 소프트웨어인지 여부에 관계없이 배포 대상 소프트웨어에 포함된 오픈소스를 모니터링한다. 오픈소스 식별 방법은 다음과 같다.

* 오픈소스 사용 요청 : 소프트웨어 개발자는 특정 제품에 오픈소스를 사용하고자 함을 오픈소스 책임자 또는 오픈소스 센터에 알리고, 검토 및 승인을 위한 오픈소스 패키지의 용도에 관한 정보를 제공한다.
* 개발 소프트웨어 검사 (Auditing) : 전체 개발 소프트웨어에 대해서도 검사를 수행하여 개발자가 임의로 복사해서 포함시킨 오픈소스를 식별한다. 
* 제3자 소프트웨어 실사 (Due diligence) : 제3자로부터 소프트웨어를 입수할 경우, 개발 소프트웨어와 통합하기 전에 검사를 수행한다. 

일련의 과정은 Jira 등 이슈 추적 시스템을 활용하여 기록한다. 

| 식별 단계 진입 조건 | 식별 단계 결과           | 
|----|-----------------|------|------|
| • 개발자로부터 특정 오픈소스 사용 요청 접수 <br>• 개발 프로세스 상 소스 코드 검사 단계<br>• 제3자 소프트웨어 입수 및 개발소프트웨어로의 통합 | • 오픈소스 사용 요청에 대한 기록 (Jira 등 활용)<br>• 소스코드 스캔 대상 선정 | 


### Step 2. 소스 코드 검사 (Auditing Source Code)

![](../step2.png)

소스 코드 검사 단계에서는 소스 코드 분석 도구를 사용하여 소스 코드를 스캔하여 오픈소스를 식별한다. 
* 소스 코드 스캔도구는 FOSSology를 이용한다. 
* 다음과 같은 라이선스 이슈가 발견될 경우, 이를 해결하도록 개발팀에 요청한다. 
  * GPL-3.0 등 정책적으로 사용할 수 없는 오픈소스 라이선스가 적용된 오픈소스 사용
  * 라이선스 충돌로 양립할 수 없는 오픈소스 사용

| 소스 코드 검사 단계 진입 조건 | 소스 코드 검사 단계 결과   | 
|----|-----------------|------|------|
| • 소스 코드 스캔 요청 (Jira ticket 생성) | • 소스 코드 스캔 결과 (오픈소스 출처, 라이선스, 저작권 등의 정보 포함)<br>• 발견된 이슈에 대해 개발팀에 해결 요청 (Jira ticket 생성) | 

### Step 3. 문제 해결 (Resolving Issues)

![](../step3.png)

소스 코드 검사 단계에서 식별된 모든 문제를 해결한다. 문제 사항은 Jira ticket으로 생성하여 개발팀에 할당되고, 오픈소스 책임자는 모든 문제가 적절하게 해결되었는지 확인한다.

| 문제 해결 단계 진입 조건 | 문제 해결 단계 결과 |
| :--- | :--- |
| • 소스 코드 스캔 완료 및 결과 생성 <br>• 문제 확인 | • 발견된 문제를 모두 해결 (Jira ticket close)|

### Step 4. 검토 (Reviews)

![](../step4.png)

발견한 모든 문제를 해결하면 검토 단계로 이동한다. 검토 단계의 절차는 다음과 같다.

1. 개발팀 PL : 소프트웨어에 포함된 모든 오픈소스를 파악하고 이에 대한 사용 승인 요청서를 Jira ticket을 생성하여 제출한다. 
2. 오픈소스 책임자 : 사용 승인 요청서를 접수하면 모든 정보가 누락 없이 포함되었는지를 확인하는 검토 절차를 진행한다. 필요 시, 법무팀에 자문을 요청한다.
3. 소스코드 검사 담당자 : 소스코드 검사를 수행하여 문제가 모두 해결되었는지 확인한다. 

| 검토 단계 진입 조건 | 검토 단계 결과 |
| :--- | :--- |
| • 발견된 모든 문제 해결 | • 승인 전 오픈소스 책임자, 소스코드 검사 담당자, 법무팀 등의 검토 완료 |

### Step 5. 승인 (Approval)

![](../step5.png)

검토가 완료되면 Jira ticket은 승인 단계로 이동한다. 오픈소스 책임자는 오픈소스의 사용을 승인하거나 거절한다. 거절 시에는 이유에 대한 설명과 수정 방법을 제안한다. 오픈소스 책임자가 오픈소스의 사용을 승인하면 개발팀은 라이선스 의무를 이행하기 위한 준비를 한다.

| 승인 단계 진입 조건 | 승인 단계 결과 |
| :--- | :--- |
| • 검토가 완료된 상태 | • 오픈소스 책임자의 오픈소스 사용 승인 혹은 거절<br>• 거절 시에는 이유에 대한 설명과 수정 방법 제안 |

### Step 6. 등록 (Registration)

![](../step6.png)

소프트웨어의 버전별 오픈소스 사용 목록을 추적하기 위한 BOM(Bill of Materials : 소프트웨어 목록)에 등록한다. BOM에는 배포 대상 소프트웨어의 버전에 포함된 오픈소스 목록과 그에 대한 다음과 같은 정보를 포함한다. 
* 배포 대상 소프트웨어의 제품 (혹은 서비스) 이름과 버전
* 오픈소스 목록 (이름 / 버전)과 해당 오픈소스 라이선스
BOM을 관리하는 도구는 SW360을 사용한다.

| 등록 단계 진입 조건 | 등록 단계 결과 |
| :--- | :--- |
| • 오픈소스 책임자가 오픈소스 사용 승인 | • BOM 등록 |

### Step 7. 고지 (Notices)

![](../step7.png)

오픈소스를 사용할 때 주요 의무 중 하나는 고지 의무이다. 이를 위해 다음 사항을 수행하기 위한 오픈소스 고지문을 작성한다. 
* 저작권, 라이선스 고지
* 오픈소스 라이선스 사본
* (해당하는 경우) 소스 코드 사본을 얻을 수 있는 서면 약정 (Written Offer)

오픈소스 고지문을 생성하면, 이를 제품/서비스 배포 시 동봉할 수 있도록 개발팀에 전달한다. 

| 고지 단계 진입 조건 | 고지 단계 결과 |
| :--- | :--- |
| • BOM 등록 | • 오픈소스 고지문 생성<br>• 오픈소스 고지문이 제품과 동봉되도록 개발팀에 전달 |

개발팀은 제품 배포 시 오픈소스 고지문을 가능한 방법을 이용하여 동봉한다. 예를 들어, 화면이 있는 제품이면 사용자가 "메뉴 > 오픈소스 고지 정보"에서 오픈 소스 고지 내용을 확인할 수 있게 오픈소스 고지문을 HTML 파일 포맷으로 포함시킨다. 제품에 화면이 없을 경우, 사용자 매뉴얼에 오픈소스 고지문 내용을 포함시킬 수 있다.

### Step 8. 배포 전 확인 (Pre-Distribution Verifications)

![](../step8.png)

이 단계에서는 공개할 소스 코드 제공을 위해 다음과 같이 소스 코드 취합 등의 활동을 수행한다. 
* 오픈소스 라이선스가 요구하는 공개할 소스 코드를 취합한다.
* 취합한 소스 코드는 제품에 탑재된 바이너리와 매치되어야 한다. 즉, 취합한 소스 코드를 빌드 했을 때 제품에 탑재된 바이너리와 동일해야 한다. 
* 소스 코드 내 부적절한 주석을 제거한다.
* 소스 코드를 직접 배포하기 곤란한 상황일 경우, 제품과 동봉한 오픈소스 고지문에 사용자에게 소스 코드를 제공하겠다는 서면 약정(Written Offer)을 포함시킨다. 

| 배포 전 확인 단계 진입 조건	 | 배포 전 확인 단계 결과 |
| :--- | :--- |
| • 오픈소스 고지문 생성| • 고지 의무를 이행할 수 있도록 조치<br>• 공개할 소스 코드 취합<br>• 소스 코드 제공 방법 결정<br>• 배포 전 확인 수행 완료


### Step 9. 배포 (Distribution)

![](../step9.png)

배포 전 확인이 완료되면 공개할 소스 코드 패키지를 오픈소스 배포사이트에 업로드한다. 최종 사용자는 자신이 원하는 제품의 버전에 해당하는 소스 코드 패키지를 오픈소스 배포사이트에서 검색하여 다운로드 받을 수 있어야 한다.

| 배포 단계 진입 조건 | 배포 단계 결과 |
| :--- | :--- |
| • 소스 코드 취합 등 모든 배포 전 확인 완료 | • 오픈소스 배포사이트에 업로드하여 사용자가 특정 제품의 버전에 대한 소스 코드 패키지를 다운로드받을 수 있게 함 |

### Step 10. 최종 확인 (Final Verifications)

![](../step10.png)

공개할 소스 코드 패키지를 오픈소스 배포사이트에 업로드 후 외부에서 오류 없이 다운로드 및 압축 해제가 되는지 확인한다. 오픈소스 라이선스가 빌드 방법까지 제공을 요구하는 경우, 외부에서 다운받은 소스 코드가 README의 안내대로 오류 없이 빌드되어 바이너리가 생성되는지, 생성된 바이너리가 제품에 탑재된 바이너리와 동일한지 확인한다.

| 최종 확인 단계 진입 조건 | 최종 확인 단계 결과 |
| :--- | :--- |
| • 오픈소스 배포사이트에 공개할 소스 코드 패키지 등록 | • 외부에서 다운로드가 이상없이 수행되는지, 제품과 동일한 버전의 바이너리와 매치가 되는지 확인 |


## 2. 외부 문의 대응 프로세스

외부로부터의 이러한 오픈소스 컴플라이언스 문의에 신속하고 정확하게 대응한다면 소송까지 진행되는 위험을 크게 줄일 수 있다. 이를 위해 기업은 외부의 오픈소스 컴플라이언스 문의에 대응하기 위해 다음과 같은 프로세스를 준수한다.

 ![process.png](../process.png) 

 _<center>< https://www.linuxsources.org/content/open-compliance-directory-add-organization-request ></center>_

 
1. 접수 확인 (Acknowledge) : 문의를 받으면 즉시 응답하여, 문의가 접수되었음을 알린다. 이때 조치 예정일을 함께 알린다. 요청자의 의도가 무엇인지 정확히 파악하는 것이 중요하기 때문에 문의가 불명확한 경우 추가 설명을 요청한다.
2. 요청자에게 알림 (Inform) : 요청자에게 오픈소스 컴플라이언스를 충실히 수행하고 있음과 요청자의 문의에 대해 조사하고 있음을 알린다. 내부 조사 진행 상황이 업데이트될 때마다 알리는 것이 좋다.
3. 내부 조사 (Investigate) : 문의에 대해 내부 조사를 진행한다. 문제가 된 제품의 버전에 대하여 컴플라이언스 프로세스가 적절하게 수행되었는지 BOM 및 문서화된 검토 이력을 통해 확인한다.
4. 요청자에게 보고 (Report) : 요청자에게 통보했던 조치 예정일 내에 내부 조사를 마치고, 이에 대한 내부 기록을 남긴 후 요청자에게 결과를 알린다.
5. 처리 종료 (Close Inquiry) : 요청자의 문의가 오해로 인한 잘못된 지적이나 요청이었다면 추가 조치 없이 요청자에게 이를 알리고 처리를 종료한다.
6. 문제 보완 (Rectify) : 내부조사에서 실제 컴플라이언스 문제가 발견되면 해당 조직은 제품 또는 서비스의 컴플라이언스 문제를 해결하기 위해 필요한 모든 절차를 수행한다. 예상되는 완료 일자를 요청자에게 다시 한번 알린다. 즉, 해당 오픈소스 라이선스의 의무를 이행하기 위한 정확한 방법과 시기를 알려야 한다. 문제를 해결한 후에는 즉시 요청자에게 알리고 문제가 해결되었음을 확인할 수 있는 최선의 방법을 제공한다.
7. 프로세스 개선 (Improve) : 컴플라이언스 문제가 있었던 경우, OSRB 미팅을 통해 사례를 검토하고, 문제가 발생한 경위를 파악하여, 문제가 재발하지 않을 수 있도록 프로세스를 개선한다.
