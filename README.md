<div align="center">
  
# ⚙️ 데이터 기반 스마트 제조 서비스 ISIX ⚙️

**대규모 투자가 제한적인 중견·중소기업을 대상으로 ML/AI 기반 SaaS Solution 지향**

<br>

<a href="http://isix.kr" style="color:black;">http://isix.kr</a>

<br>

<table align="center">
    <tr align="center">
        <td style="width:300px;"><b>vCPU</b></td>
        <td style="width:300px;"><b>RAM(GiB)</b></td>
        <td style="width:300px;"><b>CPU 크레딧/시간</b></td>
    </tr>
    <tr align="center">
        <td>1</td>
        <td>1.0</td>
        <td>6</td>
    </tr>
</table>

*AWS 웹 사양 문제로 속도가 느려질 수 있습니다.*

<br>

![isix](https://github.com/s53uni/isix-project/assets/142832376/91cc31b7-f455-4dee-9551-f0efd87fe9ae)

</div>

<br><br>

## 🙋‍♂️ Team

$I$ mplementing $S$ upply chain optimization and $I$ ndustrial automation to e $X$ pand the manufacturing industry

저희 팀은 **제조업 확장을 위한 공급망 최적화 및 산업 자동화 구현**을 목표로 하고 있는 $ISIX$ 입니다.

<br><br>

## 😀 Member

<table align="center">
    <tr align="center">
        <td style="width:300px;"><b>김소연</b></td>
        <td style="width:300px;"><b>김현준</b></td>
        <td style="width:300px;"><b>박시윤</b></td>
        <td style="width:300px;"><b>양현준</b></td>
        <td style="width:300px;"><b>이경현</b></td>
        <td style="width:300px;"><b>최예진</b></td>
    </tr>
    <tr align="center">
        <td>안정 범위 모델<br>웹 배포</td>
        <td>자동화 검사 모델<br>BE 개발</td>
        <td>생산 계획 모델<br>FE/BE 개발</td>
        <td>품질 예측 모델<br>웹 배포</td>
        <td>품질 예측 모델<br>Grafana</td>
        <td>안정 범위 모델<br>웹 배포</td>
    </tr>
</table>

<br><br>

## 🖥️ 개발환경
* Jupyter Notebook
* Visual Studio
* Sourcetree
* GitHub

<br><br>

## 🛠️ 사용기술
### Back-End
* Django
* Grafana
* MySQL

### Front-End
* HTML5
* CSS3
* Javascript

### AWS
* EC2

<br><br>

## 📌 주요기능

* 메인화면
  - 간단한 서비스 소개와 기대효과를 보여줍니다.
  - 기술 소개, 생산 계획, 공정 모니터링, 자동화 검사로 향할 수 있는 메뉴들이 있습니다.
  - 각 페이지들은 예시 데이터들로 고객이 실제 사용시 볼 수 있는 화면을 구현해두었습니다.

* 기술 소개
  - 생산 계획, 공정 모니터링, 자동화 검사에 대한 설명이 담겨있습니다.
  
* 생산 계획
  - 부품 5개에 대한 한 달의 생산 계획을 확인할 수 있습니다.
  - LSTM 모델을 사용하여 이전 정보를 오랫동안 기억할 수 있으며, 이를 통해 긴 시퀀스 데이터를 처리할 수 있습니다.
  - 딥러닝 기반의 모델로 발주 수량 예측을 확인하고 생산 계획을 수립할 수 있습니다.
  
* 공정 모니터링
  - 주조/열처리/CNC 공정에 대한 모니터링을 제공합니다.
  - 주요 특징을 식별하고 덜 중요한 특징을 무시하는 기능을 가진 XGBoost 모델을 통해 각 Feature의 값으로 제품의 품질을 예측합니다.
  - RFE 분석을 통해 주요 Feature를 도출하고 XGBoost Tree 기능으로 공정 안정 범위를 설정하였습니다.

* 자동화 검사
  - 공정이 완료된 제품의 실시간 영상을 확인할 수 있습니다.
  - YOLOv5를 이용하여 실시간 영상 중 제품을 감지하여 캡처를 진행합니다. 
  - CNN을 통해 캡처된 이미지를 양품 또는 불량품으로 예측하여 분류합니다.

💡 각 작업들은 모두 MySQLDB에 저장되며 Grafana를 통해 시각적으로 모니터링 할 수 있습니다.
