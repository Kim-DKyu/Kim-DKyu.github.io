---
layout: default
title: 이력서
---


## 학력

<div class="entry">
<div class="row"><b>아주대학교 대학원</b><time>2023.09 – 2026.02</time></div>
<p class="sub">인공지능학과 석사 · 학점 3.94 / 4.5</p>
</div>

## 논문

<div class="entry pub">
<div class="row"><b>Knowledge Distillation with Lightweight Peer Branches for Learning Diverse Representations</b></div>
<p class="sub">Scientific Reports 투고 · 1저자 · 심사 중</p>
<p class="tldr">Online KD 의 peer branch 를 경량 구조로 바꾸고 anchor 기반 loss 로 branch 간 표현을 갈라놓아, 파라미터를 늘리지 않고 표현 다양성과 앙상블 성능을 함께 얻는다.</p>
<details>
<summary>자세히</summary>
<ul>
<li>사전학습 모델 없이 스스로 증류하는 Online KD 에서 peer branch 를 마지막 stage 복제 대신 경량 네트워크로 설계해 파라미터 증가를 억제.</li>
<li>모든 peer branch logit 의 평균을 anchor 로 두고 각 branch 가 anchor 에서 멀어지도록 유도하는 loss 를 도입해 표현 다양성을 확보.</li>
<li>feature map 의 channel·spatial 분산과 앙상블 성능을 함께 비교해 표현 다양성 가설을 검증.</li>
</ul>
</details>
</div>

## 프로젝트

<div class="entry">
<div class="row"><b>복부 CT 기반 근감소증 연구 과제</b><time>2025.11 – 2026.03</time></div>
<p class="sub">아주대학교 권역외상센터 협업 · 근육량 예측 전체 프로세스 구축</p>
<p class="tldr">U-Net 으로 복부 CT 의 근육 영역을 자동 추출하고, 100장뿐인 데이터 한계를 구간화 분류로 돌려 근육량 예측 파이프라인을 끝까지 세웠다.</p>
<details>
<summary>자세히</summary>
<ul>
<li>의료진의 수작업 라벨링에서 생기는 주관적 편차와 시간 비효율 개선이 목표.</li>
<li>U-Net 을 fine-tuning 해 복부 CT 에서 근육 영역을 자동 추출하는 segmentation 모델 구축.</li>
<li>EfficientNet-B0/B1 에 regression head 를 결합해 근육량 예측 실험. 데이터 한계로 구간화 분류 문제로 재정의해 60% 달성.</li>
</ul>
</details>
</div>

<div class="entry">
<div class="row"><b>TBP 이미지 분석 SW 시스템 개발</b><time>2023.08 – 2023.12</time></div>
<p class="sub">스페클립스 산학 과제 · feature matching 알고리즘 조사 및 프로토타입 구축</p>
<p class="tldr">전신 사진 두 장에서 YOLOv8 로 점을 찾고 LightGlue 로 매칭해, 오매칭 5% 이하 · 약 2초 추론으로 생성·소멸 점을 잡는 프로토타입을 만들었다.</p>
<details>
<summary>자세히</summary>
<ul>
<li>동일 인물의 전신 이미지를 시점별로 비교해 점의 변화를 분석하고 피부암 발병 소지를 판단하는 SW 개발.</li>
<li>촬영 시점에 따른 자세·각도 변화로 픽셀 기반 매칭이 어려워, 시점 변화에 강건한 LightGlue 기반 매칭 적용.</li>
<li>bbox 크기 세 가지로 추가 실험해 중첩 구간 매칭 정확도 개선.</li>
</ul>
</details>
</div>

## 경력

<div class="entry">
<div class="row"><b>케이엘넷</b><time>2021.05 – 2022.07</time></div>
<p class="sub">인프라개발파트 연구원 · 백엔드/서버 개발</p>
<ul>
<li>선사·중계기·화주 간 문서 송수신을 위한 FTP Client/Server 운영. 이미지 BL + EDI 문서 처리 서비스 개발.</li>
<li>FTP Client/Server Kafka 통신 PDU 백업, sFTP 스레드 재기동 Poller 구축, FTP Client 신규 모듈 등록 및 유지보수.</li>
<li>통신서버 장애 우회를 위한 문서 송수신 클라우드 백업서버 구축 담당.</li>
</ul>
</div>

## 기술

<p class="chips">
<span>Python</span><span>PyTorch</span><span>OpenCV</span><span>Computer Vision</span><span>Knowledge Distillation</span>
<span>Vision-Language Model</span><span>Multimodal</span><span>Image Processing</span><span>SQL</span><span>Docker</span>
</p>

## 교육 · 자격

<div class="entry">
<div class="row"><b>코드스테이츠 AI 부트캠프</b><time>2022.08 – 2023.02</time></div>
<p class="sub">EDA · Machine Learning · SQL / Flask / Docker · 자료구조 · 알고리즘</p>
</div>

<div class="entry">
<div class="row"><b>SQL 개발자 (SQLD)</b><time>2022.12</time></div>
<div class="row"><b>정보처리기사</b><time>2020.08</time></div>
<div class="row"><b>정보처리산업기사</b><time>2019.05</time></div>
<div class="row"><b>TOEIC Speaking · Intermediate High (140)</b><time>2026.02</time></div>
</div>
