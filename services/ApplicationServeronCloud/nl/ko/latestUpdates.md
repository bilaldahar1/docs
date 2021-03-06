---

copyright:
  years: 2015, 2016

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}

# 최신 업데이트
{: #latest_updates}
마지막 업데이트 날짜: 2016년 8월 17일
{: .last-updated}

서비스에 대한 최신 업데이트 목록입니다.

## 2016년 8월 17일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}

* WebSphere Application Server for Bluemix 2진을 8.5.5.9에서 8.5.5.10으로 업그레이드했습니다.
* 다음을 포함하여 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}에 영향을 미치는 [몇 가지 보안 취약점](http://www-01.ibm.com/support/docview.wss?uid=swg21988710){: new_window}이 해결되었습니다.
  * WebSphere Application Server 및 WebSphere Application Server 하이퍼바이저 에디션 관리 콘솔에 영향을 미치는 Apache Struts 취약점
  * SIP 서비스 사용 시 IBM WebSphere Application Server의 잠재적 서비스 거부(DoS) 취약성
  * WebSphere Application Server에서 사용된 IBM HTTP Server에 영향을 미칠 수 있는 몇몇 취약점
  * IHS(IBM HTTP Server)에 영향을 미칠 수 있는 CGI 애플리케이션과 함께 HTTP 트래픽의 경로 재지정을 허용하는 취약성. 이 취약성은 "HTTPOXY"로 알려졌습니다.
  * IBM WebSphere Application Server의 정보 공개 취약성
  * webcontainer 사용자 정의 특성 HttpSessionIdReuse가 사용으로 설정되어 있는 환경에서만 발생하는 IBM WebSphere Application Server의 잠재적 우회 보안 제한 취약성


## 2016년 6월 24일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} 

* 새 *Traditional ND* 또는 *Traditional WebSphere* 인스턴스를 작성하는 경우 V8.5 및 V9.0 중에 선택할 수 있는 기능이 추가되었습니다. 
* WebSphere Application Server Liberty(Core 및 ND 플랜)의 새 인스턴스에 수정팩 16.0.0.2가 설치되도록 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} 2진이 업그레이드되었습니다. 16.0.0.2는 8.5.5.9 이후 최신 수정팩입니다. 16.0.0.2부터, 이러한 플랜을 지원하는 권한이 있는 모든 Liberty 선택 기능이 기본적으로 설치됩니다. 
* 다음을 포함하여 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}에 영향을 미치는 [몇 가지 보안 취약점](http://www-01.ibm.com/support/docview.wss?uid=swg21984977){: new_window}이 해결되었습니다. 
  * IBM WebSphere Application Server에 영향을 미치는 Apache Standard Taglibs의 XXE(XML External Entity Injection) 취약점.
  * WebSphere Application Server Liberty Profile API 검색 기능 및 Swagger 문서를 사용하는 경우 예상되는 보안보다 약한 잠재적 취약점.
  * IBM WebSphere Application Server Liberty에 대한 관리 센터의 잠재적 정보 노출 취약점.
  * IBM WebSphere Application Server의 잠재적 HTTP 응답 분할 취약점.
  * OpenSSL 프로젝트에서 2016년 5월 3일에 공개한 OpenSSL 취약점.

## 2016년 6월 13일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}

* WebSphere Application Server for Bluemix RESTful API를 사용하는 애플리케이션 또는 스크립트의 작성을 통해 클라이언트가 가상 머신 인스턴스를 빌드, 프로비저닝, 관리 및 삭제할 수 있는 기능이 추가되었습니다. 
* 클라이언트가 10개 이하의 IP 주소 또는 64GB 이하 메모리가 할당된, 고정된 수의 중지된 인스턴스를 보유할 수 있게 하는 기능이 추가되었습니다. 클라이언트는 이제 5%의 감소 비율로 중지된 상태의 누적 인스턴스에 대해 청구됩니다. 

## 2016년 4월 26일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}

* FIPS140-2가 사용되는 경우 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}의 [잠재적 보안 취약성](http://www-01.ibm.com/support/docview.wss?uid=swg21982128){: new_window} 및 Badlock을 포함한 Samba 내 다중 취약성을 해결했습니다. 
* 통합된 기타 서비스 유지보수

## 2016년 4월 15일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}

* WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} 2진 파일을 8.5.5.8에서 8.5.5.9로 업그레이드했습니다.
* OIDC(OpenID Connect) 클라이언트를 사용하는 이용자들에게 영향을 주는 IBM {{site.data.keyword.Bluemix_notm}}에 대해 Liberty for Java에서 [XSS(Cross-site scripting)](http://www-01.ibm.com/support/docview.wss?uid=swg21981221){: new_window} 취약성을 해결했습니다. 
* 통합된 기타 서비스 유지보수

## 2016년 2월 19일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}
* 해당 환경을 더 큰 가상 머신이 있는 올바른 크기로 만들도록 메모리 중심 애플리케이션이 있는 클라이언트에 대한 옵션이 추가되었습니다. 클라이언트는 최대 32GB RAM 가상 머신의 제공된 WebSphere Application Server 컴포넌트 또는 단일 시스템의 특정 리소스 크기를 선택할 수 있습니다.
* WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} 2진 파일을 8.5.5.7에서 8.5.5.8로 업그레이드했습니다.
* 일반적으로 [SLOTH](http://www-01.ibm.com/support/docview.wss?uid=swg21977244){: new_window}라고 불리는 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}에 영향을 미치는 IBM SDK Java Technology Edition에서 다중 취약성이 해결되었습니다.
* OAuth 제공자 출력의 이용자에 영향을 주는 [XSS(Cross-site scripting)](http://www-01.ibm.com/support/docview.wss?uid=swg21976337){: new_window} 취약성이 처리되었습니다.
* 통합된 기타 서비스 유지보수

## 2015년 12월 11일: 업데이트된 WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}
* 공식적인 제품 이름이 IBM Application Server on Cloud for {{site.data.keyword.Bluemix_notm}}에서 IBM WebSphere Application Server for {{site.data.keyword.Bluemix_notm}}로 변경되었습니다.
* WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} Network Deployment 플랜에 새 기능이 추가되었습니다. 플랜은 둘 이상의 가상 머신이 있는 WebSphere Application Server Network Deployment 셀 환경으로 구성됩니다. 해당 새 기능을
사용하면 고가용성, 장애 복구 및 확장성을 위한 클러스터형 환경을 설정할 수 있습니다. 
* WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} Liberty Core 플랜에 새 기능이 추가되었습니다. 플랜에는
Liberty 프로파일(서버)의 그룹에 대한 관리 도메인이고 둘 이상의
가상 머신으로 구성된 Liberty Collective의 사용이 포함됩니다. 
* WebSphere Application Server for {{site.data.keyword.Bluemix_notm}} 2진 파일을 8.5.5.6에서 8.5.5.7로 업그레이드했습니다.
* Java 오브젝트 직렬화 해제를 처리하기 위한 [Apache Commons Collections
취약성](https://www.us-cert.gov/ncas/current-activity/2015/11/13/Apache-Commons-Collections-Java-Library-Vulnerability){: new_window}이 처리되었습니다.
* [HTTP 응답 분할 공격](http://www-01.ibm.com/support/docview.wss?uid=swg21972254){: new_window}을 허용하는 취약성이
처리되었습니다.
* 통합된 기타 서비스 유지보수

## 2015년 10월 15일: 업데이트된 Application Server on Cloud
* 다음 2개의 새로운 플랜이 추가되었습니다.
  * [WebSphere Application Server Traditional V9 Beta](https://www-01.ibm.com/marketing/iwm/iwmdocs/web/cc/earlyprograms/websphere.shtml){: new_window}
  * WebSphere Application Server ND
* 기타 서비스 유지보수