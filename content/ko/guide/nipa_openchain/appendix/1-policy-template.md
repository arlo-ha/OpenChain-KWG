---
title: "1. 샘플 오픈소스 정책"
weight: 1
type: docs
---
{{< alert title="Note:" >}}
이 샘플 오픈소스 정책은 다음 두 가지 자료를 참고하여 작성하였다.

1. [OpenChain Open Source Policy Template](https://github.com/OpenChain-Project/Reference-Material/blob/master/Open-Source-Policy/Official/2.1/en/Open-Source-Policy-Template-en-OpenChain2.1-ISO5230.xlsx)
2. [Linux Foundation Generic FOSS Policy](https://github.com/todogroup/policies/blob/master/linuxfoundation/lf_compliance_generic_policy.pdf)
{{< /alert >}}


## 오픈소스 정책

### 1. 목적

이 정책은 오픈소스를 사용하는 조직 전체가 오픈소스 컴플라이언스 활동을 수행하도록 수립되었다. 이 정책은 모든 구성원이 오픈소스의 가치를 이해하고, 오픈소스를 올바르게 사용하며, 오픈소스 커뮤니티에 기여하기 위한 방법을 제공한다.

이 정책은 모든 구성원이 오픈소스 정책을 쉽게 접할 수 있도록 내부 시스템인 [LINK]에서도 확인할 수 있다.

### 2. 적용 범위

이 정책은 다음 세 부분에 적용한다. 
1. [회사가 외부로 제공하거나 배포하는 모든 제품]에 적용한다. 단, 오픈소스를 내부 사용 목적으로만 사용하는 것은 이 정책의 범위에 포함되지 않는다.
2. 구성원이 외부 오픈소스 프로젝트로의 기여 시에 적용한다.
3. 내부 코드를 오픈소스로 공개할 때 적용한다.


### 3. 용어

"컴플라이언스 산출물" - 컴플라이언스 프로그램의 결과물을 의미한다. 배포용 소프트웨어 공급 시 함께 제공해야 하는 산출물의 모음이다. 여기에는 다음 사항이 포함된다(단, 이에 국한되지 않음) : 저작자 고지, 소스 코드, 빌드 및 설치 스크립트, 라이선스 사본, 저작권 고지, 수정 내용 고지, 서면 청약(Written Offer), 오픈소스 컴포넌트 BOM (Bill of Materials), SPDX 문서.

"오픈소스" - Open Source Initiative에서 만든 Open Source Definition (opensource.org/osd) 혹은 Free Software Foundation에서 만든 Free Software Definition (gnu.org/philosophy/free-sw.html)을 충족하는 라이선스, 혹은 이와 유사한 라이선스가 하나 이상 적용된 소프트웨어이다.

"오픈소스 프로그램" - 오픈소스 정책, 프로세스, 인원 등 기업이 오픈소스 컴플라이언스 활동을 수행하기 위한 일련의 관리 체계를 의미한다.

"배포용 소프트웨어" : 기업이 제3자(예: 다른 조직 또는 개인)에게 배포하는 소프트웨어이다. 

"OpenChain 프로젝트" - Linux Foundation의 프로젝트이며 오픈소스 컴플라이언스를 위한 국제 표준으로써 기업이 오픈소스 컴플라이언스를 위해 준수해야 할 활동을 더 간단하고 일관성 있게 만들어 소프트웨어 공급망 전체에 신뢰를 구축하기 위한 활동을 한다. 

"OpenChain 적합성" - 기업의 오픈소스 활동이 OpenChain 규격의 모든 요구 사항을 준수함을 의미한다. 


### 4. 역할, 책임 및 역량

이 장에서는 이 정책의 효과적인 수행을 보장하기 위해 다음과 같이 필요한 역할 및 책임과 각 역할의 담당자가 갖추어야 할 역량을 정의한다. 
* 소프트웨어 개발 및 배포를 담당하는 임원은 오픈소스 프로그램의 각 역할을 위한 담당자를 지정하고, 역할을 수행할 적절한 시간과 예산이 할당되도록 보장해야 한다.
* 각 역할의 담당자는 자신이 역할을 수행하면서 적절한 지원이 되지 않는다면 반드시 오픈소스 책임자에게 문제를 제기해야 한다. 적절하게 해결되지 않는다면, OSRB에 문제 해결을 요청해야 한다.

#### 가) 오픈소스 책임자

오픈소스 책임자는 기업의 오픈소스에 대한 총괄 책임을 담당하며, 오픈소스 센터를 설립하고 운영하며,  OSRB를 주관한다. 오픈소스를 사용한 제품과 서비스의 오픈소스 컴플라이언스를 보장하기 위해 다음 사항에 대한 책임이 있다.

* 오픈소스 정책을 검토, 개선 및 전파한다.
* 오픈소스 정책을 효율적으로 수행하기 위해 회사 내부에 역할을 지정하고, 책임을 할당한다.
* 오픈소스 컴플라이언스 교육을 주관하고 평가한다.
*  OSRB의 의장을 맡아서 활동을 지휘한다.
* 소프트웨어 개발팀이 오픈소스 정책과 프로세스를 이해하고 준수하도록 안내한다. 필요할 경우 경영진에게 문제를 제기하여 해결한다.
* 외부로부터의 오픈소스 사용 및 컴플라이언스에 대한 문의에 신속히 답변한다.

이를 위해 오픈소스 책임자에게 필요한 이해와 역량은 다음과 같다. 
* 소프트웨어 개발 프로세스
* 저작권, 특허 등 오픈소스 라이선스와 관련한 지식재산
* 오픈소스 컴플라이언스에 대한 전문 지식
* 오픈소스 개발 경험
* 커뮤니케이션 스킬

2020년 1월 현재 OOO팀의 OOO가 오픈소스 책임자 역할을 담당한다.

#### 나) 오픈소스 센터

오픈소스 센터는 오픈소스 컴플라이언스를 위한 전문 센터이며, 컴플라이언스를 효과적으로 달성하기 위한 프로세스를 정의한다. 오픈소스 책임자가 리더 역할을 수행하고, 센터의 구성원들은 오픈소스 책임자가 원활하게 책임을 수행할 수 있도록 돕는 역할을 맡는다. 오픈소스 센터는 다음과 같은 역할을 수행한다.

* 컴플라이언스 실무 교육을 개발 및 제공한다.
* 컴플라이언스를 위한 자동화 도구를 선택 / 개발 및 제공한다.
* 코드 스캔 및 검사를 수행하여 제품과 서비스 내 오픈소스를 식별한다.
* 오픈소스 사용 요청을 검토하고 승인한다.
* 오픈소스 사용 목록(BOM)에 관한 기록을 유지한다.
* 오픈소스 고지 및 소스코드 공개를 위한 웹사이트를 개발하고 유지 관리한다.

오픈소스 센터의 구성원에게 필요한 이해와 역량은 다음과 같다. 
* 소프트웨어 개발 프로세스
* 저작권, 특허 등 오픈소스 라이선스와 관련한 지식재산
* 오픈소스 컴플라이언스에 대한 기본 지식
* 오픈소스 컴플라이언스 도구 활용 능력

#### 다)  OSRB

OSRB(Open Source Review Board)는 오픈소스 운영위원회라고도 불리며, 기업의 오픈소스 관리를 위해 오픈소스 매니저와 법무팀, 특허팀, 개발팀, 인프라팀 등 관련 조직의 담당자로 구성된 협의체이다. 
* OSRB는 오픈소스 관리를 위한 정책과 프로세스를 만들고, 이를 수행하기 위한 기업 내의 R&R을 정의한다. 
* 기업 내 오픈소스 관리 이슈 발생 시, 해결 방안을 논의하고, 대응 방안을 마련한다.
* 필요 시, 임원진에 이슈를 보고하여 리스크 완화 방안에 대한 피드백을 받는다. 

 OSRB의 구성원에게 필요한 이해와 역량은 다음과 같다. 
* 소프트웨어 개발 프로세스
* 오픈소스 컴플라이언스에 대한 기본 지식 

#### 라) 소프트웨어 개발팀

소프트웨어 개발팀은 기업의 오픈소스 정책 및 프로세스를 충분히 이해하고, 다음 사항을 준수한다. 
* 소프트웨어 개발에 사용할 오픈소스를 식별하고 오픈소스 센터에 오픈소스 사용 승인 요청을 제출한다.
* 소프트웨어 개발에 사용한 오픈소스에 적용되는 오픈소스 라이선스의 의무를 이행한다. 
* 오픈소스의 결합 관계를 파악하여 자사의 코드가 오픈소스 라이선스의 영향을 받지 않도록 소프트웨어 아키텍처를 설계한다. 

소프트웨어 개발팀의 구성원에게 필요한 이해와 역량 역량은 다음과 같다. 
* 소프트웨어 개발 프로세스
* 오픈소스 컴플라이언스에 대한 기본 지식 

#### 마) 법무팀

법무팀은 오픈소스 라이선스와 의무를 해석한다. 이러한 의무를 실제 이행하기 위해 가이드를 소프트웨어 개발팀에 제공하고, 필요에 따라 다음 사항을 수행한다. 
* 호환되지 않는 오픈소스 라이선스로 인한 충돌을 포함하여 라이선스 및 지식재산권 문제에 대해 자문을 제공한다. 
* 오픈소스 사용 검토 및 승인 결정에 참여한다.
* 외부 오픈소스 프로젝트로의 기여를 위한 검토 요청에 의견을 제공한다.

법무팀의 구성원에게 필요한 이해와 역량은 다음과 같다. 
* 오픈소스 생태계에 대한 기본 지식
* 소프트웨어 저작권에 대한 전문 지식
* 오픈소스 라이선스에 대한 전문 지식


### 5. 교육 및 평가

#### 교육

오픈소스 책임자는 프로그램 참여자를 대상으로 매년 혹은 2년에 한 번씩 주기적인 교육을 제공함으로 모든 프로그램 참여자가 오픈소스 정책의 존재와 다음 사항을 인식하게 한다. 

(1) 오픈소스 정책의 존재 및 목표

(2) 구성원 기여 방법
* 모든 구성원은 이 정책의 근거와 내용을 이해하고 필요한 활동을 충실히 수행함으로써 정책의 효과 및 회사의 컴플라이언스 수준 향상에 기여할 수 있다. 

(3) 미준수 시 위험 사항
* 사용 중인 코드에 대한 저작권 또는 기타 지식재산권 보유자의 법적 클레임
* 고객으로부터의 클레임
* 회사 독점 코드의 의도치 않은 공개
* 라이선스 의무 위반으로 인한 벌금 부과
* 평판 손실
* 수익 손실
* 공급업체 및 고객과의 계약 위반
이러한 이유로 회사는 코드 침해를 심각하게 간주하며, 코드를 침해하는 개인은 회사의 징계 절차에 처할 수 있다.

신규 입사자 대상 교육 시 오픈소스 정책에 대한 교육을 의무화한다. 또한, 누구나 수시로 오픈소스 정책을 참고할 수 있도록 사내 Wiki를 통해 전파한다.


#### 평가

이 정책을 수행하는 모든 참여자는 자신의 역할에 필요한 역량을 다루는 최소한의 기본 교육을 수강하고 평가를 받는다. 기업은 교육 제공과 평가를 통해 모든 참여자가 각자 자신의 역할을 수행할 역량을 갖추었음을 보장한다. 

평가 기록은 최소 3년 동안 유지한다.


### 6. 오픈소스 사용 정책

소프트웨어 개발에 오픈소스를 사용하기 위해 소프트웨어 개발팀은 다음 사항을 준수한다. 
* 먼저 오픈소스 라이선스가 무엇인지 식별하고, 라이선스가 요구하는 의무 사항을 검토하고 확인한다. 
* 그렇게 배포용 소프트웨어에 포함된 오픈소스와 라이선스 의무사항을 식별하고, 소프트웨어를 배포 시 라이선스 의무사항을 준수하기 위한 활동을 수행하여 컴플라이언스 산출물을 생성한다.
* 배포용 소프트웨어에 포함된 오픈소스 현황(BOM : Bill of Materials)을 문서화하여 관리한다. 
* 이를 효과적으로 수행하기 위해 기업의 오픈소스 컴플라이언스 프로세스를 준수한다.

오픈소스 라이선스를 준수하는 과정에서 의문사항이 있을 경우 소프트웨어 개발팀은 오픈소스 센터에 문의한다. 
* 일반적이지 않은 사용 사례여서 법적 해석이 명확하지 않을 경우, 오픈소스 센터는  법무팀에 문의 할 수 있다.
* 오픈소스 사용에 대한 검토 결과 및 관련 근거는 오픈소스 이슈 추적 시스템에 기록한다.


### 7. 외부 문의 대응 정책

#### 연락처 공개

기업은 외부에서 오픈소스 관련한 문의 및 요청을 할 수 있도록 담당자의 연락처를 공개적으로 제공한다. 
* 이를 위해 소프트웨어 배포 시 오픈소스 센터의 이메일 주소를 제공한다. 
* 또한, Linux Foundation의 Open Compliance Directory ([https://compliance. linuxfoundation.org/ references/open-compliance-directory/](https://compliance.linuxfoundation.org/references/open-compliance-directory/))에 오픈소스 센터의 연락처를 등록한다.

#### 외부 문의 대응 절차

 공개한 연락처로 외부 문의가 접수된 경우, 오픈소스 센터는 즉시 문의를 검토하여 기업 내 적절한 개인 또는 조직에 할당한다. 이를 위한 세부 절차는 다음과 같다. 

1. 질의 접수 승인 및 적절한 해결 시간을 명시한다.
2. 질의가 진짜 문제인지를 확인한다. (아니라면 영업일 기준 3일 이내에 질의자에게 응답한다.)
3. 이슈가 진짜 문제라면, 3일 이내에 적절한 대응 방법을 결정하고, 질의자에게 대응 계획에 대해 응답한다.
4. 결정한 방법에 따라 30일 이내에 대응하고, 질의자에게 문제가 해결되었음을 알린다.
5. 이상의 사항을 오픈소스 이슈 추적시스템에 기록한다.

이러한 외부 문의를 할당하고 처리하는 것에 대한 전반적인 책임은 오픈소스 책임자에게 있다. 

기업 내 누구든지 외부로부터 오픈소스 관련 문의를 받은 경우, 즉시 오픈소스 센터에 전달하여 외부 문의가 신속히 처리될 수 있도록 한다. 

### 8. 오픈소스 기여 정책

기업은 오픈소스에서의 비즈니스 가치 창출을 위해 외부 오픈소스 프로젝트로의 참여와 기여를 권장한다. 그러나 이 과정에서 의도하지 않은 기업의 지식 재산 노출 혹은 제3자의 권리 침해에 주의해야 한다. 이를 위해 기업의 구성원이 외부 오픈소스 프로젝트로의 기여를 위해서는 다음 사항을 준수해야 한다.
* 회사의 업무와 관련이 있는 오픈소스 프로젝트에 기여하기 위해서는 먼저 SW개발팀 리더에게 승인을 받아야 한다.
* 외부 오픈소스 프로젝트에 최초 기여 시에는 오픈소스 센터에 이를 알린다. 
* 오픈소스 센터는 오픈소스 프로젝트의 오픈소스 라이선스와 특허 조건을 검토한다. 그리고, 오픈소스 프로젝트가 DCO (Developer Certificate of Origin), CLA (Contributor License Agreement) 등에 서명을 요구할 경우 에 대해 검토해야 한다. 필요할 경우 법무팀에 검토를 요청할 수 있다.

### 9. OpenChain 적합성

기업은 소프트웨어 공급망에서의 오픈소스 컴플라이언스 수준 향상을 위해 Linux Foundation의 OpenChain 프로젝트의 정신을 지지하며 적극적으로 참여한다. 또한 기업은 다음 사항을 확약한다.

* 이 오픈소스 정책은 OpenChain 규격 버전 2.1에 적합하도록 설계되었다.
* 기업은 OpenChain 규격 버전 2.1의 모든 요구사항을 준수한다. 
* 기업은 OpenChain 적합성을 선언한 이후 최소 18개월 이상 OpenChain 규격 버전 2.1의 모든 요구사항을 준수하기 위해 정책 및 프로세스를 계속 개선하며 유지한다.
