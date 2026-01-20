# 🖱️ BodyClick

**몸을 클릭하는 순간, 건강 해답이 시작됩니다.**

BodyClick은 **3D 인체 모델과 장기 인터랙션**을 기반으로
사용자가 **몸을 직접 클릭하며 증상을 입력**하고,
AI 분석을 통해 건강 정보를 탐색할 수 있는 **인터랙티브 헬스케어 웹 서비스**입니다.

복잡한 텍스트 입력이나 의료 용어 없이,
**사람의 몸과 장기를 직접 누르는 UX**로
누구나 직관적으로 자신의 상태를 표현할 수 있습니다.

---

## 🧍 Core UX: 3D Human & Organ Interaction

**BodyClick의 핵심은 UI입니다.**

* 🧍 **3D 사람 모델 기반 인터페이스**
* 🫀 **장기 단위 클릭 인터랙션 (심장, 폐, 위 등)**
* 🎯 클릭 위치에 따라 **컨텍스트가 달라지는 AI 분석**
* 📍 “어디가 불편한지”를 **말이 아닌 행동으로 표현**

> **말로 설명하지 마세요.
> 몸을 클릭하세요.**

---

## ✨ Why BodyClick?

### 🔥 1. 텍스트 없는 입력 방식

* 의료 용어를 몰라도 사용 가능
* 노약자·비전문가에게도 직관적인 UX

### 🧠 2. RAG 기반 AI 분석

* 단순 LLM 호출 ❌
* 내부 도메인 데이터를 조회한 뒤 응답 생성 ⭕

### 🎨 3. 시각 중심 인터랙션

* 기존 헬스 서비스와 완전히 다른 접근
* “읽는 서비스”에서 “조작하는 서비스”로 전환

---

## 🤖 AI Architecture (RAG)

BodyClick의 AI는 **RAG(Retrieval-Augmented Generation)** 구조를 사용합니다.

1. 사용자가 **3D 인체 또는 장기를 클릭**
2. 서버에서 **관련 도메인 데이터 조회 (Supabase)**
3. 조회된 컨텍스트를 프롬프트에 결합
4. **Gemini API**를 통해 응답 생성

이를 통해 **내 몸의 위치와 맥락을 이해하는 AI 응답**을 제공합니다.

---

## 🏗️ System Architecture

* **Frontend**: React (Next.js)
  → 3D 인체/장기 인터랙션 UI
* **Server**: Next.js Server
  → Server-Side Rendering (SSR), API Routes
* **Authentication**: NextAuth.js
  → Session-based Auth, Google OAuth
* **Database**: Supabase (Managed PostgreSQL)
* **ORM**: Prisma
* **AI**: Gemini API (RAG-based)
* **Infrastructure**: AWS EC2 Runtime Environment

<p align="center">
  <img 
    src="https://raw.githubusercontent.com/ORG_OR_USER/BodyClick-FE/main/bodyclick/assets/BodyClick_architecture.png"
    alt="BodyClick System Architecture"
    width="850"
  />
</p>

> **Figure.** Overall system architecture of BodyClick, including Next.js full-stack application,  
> session-based authentication, RAG-based AI pipeline, and external services.

---

## 🚀 Key Features

* 🧍 3D 인체 모델 기반 증상 입력
* 🫀 장기 단위 클릭 인터랙션
* 🧠 RAG 기반 AI 건강 분석
* 🗺️ Kakao Map API 연동
* 🔐 Google OAuth 로그인
* ⚡ SSR 기반 빠른 응답

---

## 🎯 Vision

BodyClick은
“의료 정보를 읽는 서비스”가 아니라,
“몸을 직접 다루며 이해하는 서비스”를 목표로 합니다.

> **클릭 한 번으로,
> 내 몸을 더 잘 이해하다.**

---

## 📎 Tech Stack

| Category      | Technology                     |
| ------------- | ------------------------------ |
| UI / Frontend | React, Next.js, 3D Interaction |
| Backend       | Next.js (API Routes, SSR)      |
| Auth          | NextAuth.js, Google OAuth      |
| Database      | Supabase (PostgreSQL)          |
| ORM           | Prisma                         |
| AI            | Gemini API (RAG)               |
| Infra         | AWS EC2                        |

---

## 👥 Our Team

| Name | Affiliation | Role |
|---|---|---|
| **신원영** | Dept. of Information System, Hanyang University | Frontend Developer |
| **최영운** | School of Computing, Kaist | Backend Developer |
