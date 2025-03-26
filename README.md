# RAG_ChatBot
대한민국 현행법령을 기반으로 한 RAG 챗봇 소스 코드입니다

## 사용 기술
- **LLM**: EEVE-Korean-Instruct-10.8B
- **Retriever**: jina-embedding-v3 기반 dense retriever
- **Reranker**: BAAI/bge-reranker-base
- **문서 구성**: 대한민국 현행법령(법률, 시행령, 시행규칙) 약 5,800건 기반 vector DB 구축
- **전처리**: 문서별 조문 단위 chunk, 메타데이터 tagging

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


### 1. file_lodaer.ipynb - pdf 파일 로딩 테스트
### 2. embedding.ipynb - chroma 벡터 임베딩, jina-embedding 테스트
### 3. generaotr.ipynb - LLM generator lm-studio 연결 및 langchain 연결 답변 생성 테스트, prompt engineering
### 4. elasticSearch_test.ipynb - elasticSearch를 활용한 BM25 + knn Hybrid Search 테스트 (검색 결과 불만족으로 폐기)
### 5. model_score_checj.ipynb - 최종 모델로 답변 생성
