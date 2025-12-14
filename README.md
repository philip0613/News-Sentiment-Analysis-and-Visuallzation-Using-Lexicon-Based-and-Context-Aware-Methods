# News-Sentiment-Analysis-and-Visuallzation-Using-Lexicon-Based-and-Context-Aware-Methods
졸업심화연구




본 연구는 Python 기반 자동화 스크립트를 통해 네이버 뉴스의 정치, 경제, 사회, 생활, 세계, IT/과학 기사 URL과 본문을 대량 수집하고, 텍스트 마이닝과 감성 분석을 결합한 분석 파이프라인을 구축하였다. requests, BeautifulSoup로 날짜/카테고리/페이지를 입력받아 크롤링하며, 모바일 URL을 데스크톱 본문 URL로 변환하는 모듈을 구현했다. 수집 텍스트는 정규표현식 전처리 후 형태소 분석(Okt)으로 명사를 추출하고 불용어, 숫자, 1글자 토큰을 제거하였다. 이후 단어 빈도를 Counter, pandas로 집계해 상위 키워드와 워드클라우드를 시각화했다. 감성 분석은 KNU SentiLex 사전 기반 점수화와 함께 KoELECTRA 문맥 기반 분류를 추가하여, 긴 문서에 대해 truncation(max_length=512)으로 안정적으로 확률/점수를 산출하고 분포(히스토그램) 및 평균을 비교 분석하였다. 이를 통해 핵심 이슈와 정서적 편향을 신속히 정량화하는 도구를 제안한다.
