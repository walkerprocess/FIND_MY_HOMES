<img src="https://capsule-render.vercel.app/api?type=waving&color=BDBDC8&height=150&section=header" />

# 🏠 Find My Home: Public Rental Housing Information Assistant

...

# 🏠 찾아줘 홈즈: 공공임대주택 정보 안내 도우미 / Find My Home: Public Rental Housing Information Assistant

**찾아줘 홈즈**는 공공임대주택 정보를 쉽고 빠르게 찾을 수 있도록 도와주는 AI 기반 챗봇 서비스입니다.  
사용자의 나이, 혼인 여부, 지역 등의 정보를 기반으로 맞춤형 공고를 추천하며,  
카카오톡을 통해 손쉽게 이용할 수 있도록 구현되었습니다.

**Find My Home** is an AI-powered chatbot service designed to help users easily search for public rental housing information in Korea.  
Based on the user's age, marital status, and region, it recommends customized housing notices.  
It is conveniently accessible through KakaoTalk.

---

## 📌 프로젝트 개요 / PROJECT OVERVIEW

- **목표:** 공공임대주택 관련 정보를 사용자 맞춤형으로 제공하여 정보 접근성을 향상시키고 복잡한 주거 지원 정보를 쉽게 전달.
- **기능 요약:**

  - 사용자 정보 기반 맞춤형 공고 추천
  - 지역별 공고 검색
  - 카카오톡 챗봇 UI 제공
  - RAG 기반 LLM을 활용한 자연어 질의 응답
  - 인공지능 윤리 적용

- **Goal:** Improve accessibility to public rental housing information by offering personalized recommendations and simplifying complex housing policies.
- **Key Features:**
  - Personalized notice recommendations based on user profile
  - Regional notice search
  - Chatbot interface on KakaoTalk
  - RAG-based LLM (GPT-4) for natural language Q&A
  - Ethical AI considerations

---

## 프로젝트 기획 / OVERALL PLANNINGS

- **기획 & 데이터 분석:** 정책 자료 수집, 전처리 설계
- **백엔드 개발:** Flask 서버, RAG 파이프라인 구축
- **프론트/챗봇 개발:** 카카오톡 챗봇 UI, 사용자 응답 흐름 구성
- **LLM 응답 최적화:** Query Rewriting, Prompt Engineering

- **Planning & Data Analysis:** Policy document collection, preprocessing design
- **Backend Development:** Flask server, RAG pipeline
- **Frontend/Chatbot:** KakaoTalk chatbot UI, user flow design
- **LLM Optimization:** Query rewriting, prompt engineering

---

## 🗂️ 사용 기술 스택 / TECH STACK

- **LLM:** OpenAI GPT-4 (Azure AI)
- **RAG:** Azure Cognitive Search + Custom Embedding
- **백엔드:** Python, Flask, ngrok
- **챗봇:** Kakao i Open Builder 연동
- **데이터 전처리:** pandas, PyMuPDF, PDFMiner
- **인프라:** Azure Functions, Azure Blob Storage

- **LLM:** OpenAI GPT-4 (Azure AI)
- **RAG:** Azure Cognitive Search + Custom Embeddings
- **Backend:** Python, Flask, ngrok
- **Chatbot:** Kakao i Open Builder integration
- **Preprocessing Tools:** pandas, PyMuPDF, PDFMiner
- **Infrastructure:** Azure Functions, Azure Blob Storage

---

---

## 📚 데이터셋 및 처리 방식 / DATASET AND PROCESSING

- **데이터 출처:** 공공임대주택 공고문 PDF 자료 /LH, GH, SH
- **처리 내용:**

  - 제목 수준 구분 및 표 구조 추출
  - Chunk 기반 분할 및 임베딩
  - BM25 + HNSW 인덱싱
  - LLM 연결을 위한 Prompt 템플릿 구성

- **Source:** PDF documents of public rental housing announcements / LH, GH, SH
- **Process:**
  - Title-level chunking and table structure extraction
  - Text chunking and embedding
  - BM25 + HNSW indexing
  - Prompt templating for LLM integration

---

## 💬 챗봇 기능 시나리오 / CHATBOT SCENARIOS

### 1. 지역 기반 공고 찾기

> "서울에 있는 공공임대주택 뭐 있어?"

### 2. 맞춤형 공고 추천

> "30대 미혼 남성인데 경기도에서 신청 가능한 공고 알려줘."

### 1. Regional Notice Search

> "What public rental housing is available in Seoul?"

### 2. Personalized Recommendation

> "I’m a single man in my 30s living in Gyeonggi-do. What housing options can I apply for?"

---

## 🛠️ 향후 개선 방향 / FUTURE IMPROVEMENTS

- 자연어 질문 다양성 대응력 향상
- 타 플랫폼(예: 네이버톡, 웹앱) 연동
- 이미지 기반 공고문 요약 기능 추가

- Enhanced support for diverse natural language queries
- Multi-platform support (e.g., NaverTalk, WebApp)
- Visual summarization of document content (image to text)

## 더 자세한 내용은 첨부된 pdf 파일을 확인해 주세요! / FOR MORE INFORMATION PLEASE CHECK THE PDF FILE
