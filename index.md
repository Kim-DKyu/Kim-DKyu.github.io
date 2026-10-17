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
<p class="authors"><strong>Dongkyu Kim</strong><sup>†</sup>, Soohyun Pyo<sup>†</sup>, Junhyeong Go, Jongbin Ryu <span class="note">(<sup>†</sup> equal contribution)</span></p>
<p class="sub">Scientific Reports · 2차 수정(revision) 중 · Ajou University</p>
<p class="plinks"><a href="https://github.com/Kim-DKyu/DLPB">Code</a><a href="https://doi.org/10.5281/zenodo.22761858">Zenodo</a></p>
<p class="tldr">Online KD 에서 백본 stage 를 복제하던 peer branch 를 공유 stage 위의 경량 branch(DLPB) 로 바꾸고, branch 평균을 anchor 로 둔 decorrelation loss 로 서로 다른 예측을 내게 해, 추론 비용 증가 없이 CIFAR-100 ResNet32 +3.94%p, ImageNet-1K ConvNeXt +0.53%p · CSWin +0.77%p 를 얻었다.</p>
<details>
<summary>자세히</summary>
<ul>
<li>문제: 기존 multi-view online KD 는 백본 stage 일부를 복제해 peer branch 를 만들어, branch 수에 따라 파라미터가 선형으로 늘고 branch 간 출력이 비슷해지는 표현 중복이 생김.</li>
<li>구조: 각 stage 의 multi-scale feature 를 모아 하나의 공유 peer stage 에 넣고, 그 위에 경량 블록으로 여러 peer branch 를 둠. branch 는 학습에만 쓰고 추론 때 제거해 모델 크기와 속도는 baseline 과 동일.</li>
<li>학습: peer branch logit 평균의 softmax 를 anchor 분포로 정의하고, 각 branch 가 anchor 에서 멀어지도록 하는 decorrelation loss 를 도입해 표현 다양성을 유도.</li>
<li>검증: CIFAR-100 (ResNet32/110, WRN20-8/40-2, DenseNet40) 과 ImageNet-1K (ResNet18, RSB-ResNet50/101, ConvNeXt, CSWin) 에서 일관된 향상. 2026년 최신 방법(ICOKD, HSKD)과 동일 프로토콜로 비교.</li>
<li>분석: t-SNE, Grad-CAM, feature 분산으로 branch 들이 실제로 다른 표현 공간에 활성화됨을 확인하고 앙상블 성능과의 관계를 제시.</li>
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
