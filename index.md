---
layout: default
title: 이력서
---

# 김동규

<p class="lead">초분광 영상(HSI) AI 연구원 · 파운데이션 모델 · 전이학습 플랫폼</p>
<p class="contact"><a href="https://github.com/kim-dong-kyu123">github.com/kim-dong-kyu123</a><a href="mailto:you@example.com">you@example.com</a><a href="resume.pdf">PDF</a></p>

## 경력

<div class="entry">
<div class="row"><b>○○연구소</b><time>2024.03 – 현재</time></div>
<p class="sub">연구원 · 초분광 영상 AI</p>
<ul>
<li>초분광 전이학습 플랫폼(hsi-platform) 설계·개발. 동결 백본 위에 태스크 헤드만 튜닝하는 구조. FastAPI + React.</li>
<li>이미지 단위 라벨 세트 묶음 점검 기능 개발. 1,152장 검증에서 재현율 90%, 오탐 16%.</li>
<li>MLflow 기반 백본 가중치 적재와 온프레미스 GPU 서버 배포 파이프라인 구축.</li>
</ul>
</div>

## 프로젝트

<div class="entry">
<div class="row"><b>hsi-platform</b><time>2026</time></div>
<p class="sub">초분광 전이학습 플랫폼</p>
<ul>
<li>mrmae / hyper-focus 두 백본을 하나의 임베딩 인터페이스로 캡슐화. 백본을 바꿔도 하위 계층은 그대로.</li>
<li>캐시·데이터 파이프라인·헤드 학습·평가·가드레일을 Mock 백본으로 CI에서 검증.</li>
</ul>
</div>

<div class="entry">
<div class="row"><b>KFRI-SpiceGrade</b><time>2026</time></div>
<p class="sub">향신료 등급 판정 현장 앱</p>
<ul>
<li>PySide6 데스크톱 앱. v71 픽셀 인코더 + deep-sets 풀링으로 컨베이어 캡처 영상을 실시간 판정.</li>
</ul>
</div>

## 기술

<p class="chips">
<span>Python</span><span>PyTorch</span><span>FastAPI</span><span>React</span><span>TypeScript</span>
<span>MLflow</span><span>Docker</span><span>SQLite</span><span>Hyperspectral</span><span>Self-supervised</span>
</p>

## 학력

<div class="entry">
<div class="row"><b>○○대학교</b><time>2018 – 2024</time></div>
<p class="sub">○○학과 학사</p>
</div>
