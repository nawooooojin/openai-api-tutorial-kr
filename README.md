# 🤖 LLM API Hands-on

**OpenAI API로 배우는 LLM API 실습 (한국어)**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-GPT--6-412991?logo=openai&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-ready-F9AB00?logo=googlecolab&logoColor=white)
![Last Updated](https://img.shields.io/badge/updated-2026.10-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

아주대학교 「모바일컴퓨팅특론」 수업에서 LLM API 실습을 진행하면서 만들었던 자료를 정리해서 공개합니다.
텍스트 생성부터 Function Calling, 이미지·음성 생성, 그리고 **유튜브 강의를 PDF 요약본으로 만들어주는 미니 프로젝트**까지, Colab에서 바로 돌려볼 수 있게 구성했어요.

<br>

## 👋 소개

원래 2025년 11월에 **GPT-5 API** 기준으로 만든 실습인데, 수업 끝나고 묵혀두기엔 좀 아까워서 공개하게 됐습니다.
그 사이에 OpenAI API가 생각보다 많이 바뀌어서, **2026년 10월 기준 최신 API(GPT-6, gpt-image-2.5, gpt-transcribe 등)로 전부 업데이트**하고 강의·정답 노트북은 전부 다시 실행해서 결과까지 채워뒀어요.

이런 분들께 추천합니다.

- 🐣 LLM API를 처음 써보는 분
- 🧑‍💻 GPT-5 시절 코드를 최신 API로 옮기려는 분
- 🧑‍🏫 LLM API 실습 수업 자료가 필요한 분 (그대로 가져다 쓰셔도 돼요!)

도움이 됐다면 ⭐ 하나 눌러주시면 저는 기분이 좋습니다 😆

<br>

## 📚 커리큘럼

✍️ 표시는 빈칸을 직접 채워보는 **실습 노트북**이고, 정답은 [`Practice_solution/`](Practice_solution/)에 있습니다.

### Part 1. Text Generation 📘

| 노트북 | 내용 | |
| --- | --- | --- |
| [00 · OpenAI API Quick Start](1_Text_Generation/00-OpenAI%20API%20Quick%20Start.ipynb) | Responses API 첫 호출, 이미지 입력, 웹 검색 도구, 스트리밍 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/1_Text_Generation/00-OpenAI%20API%20Quick%20Start.ipynb) |
| [01 · Text Generation](1_Text_Generation/01-Text%20Generation-Lecture.ipynb) | 주요 파라미터, GPT-6 모델 비교, `reasoning.effort` / `text.verbosity`, 메시지 역할, 멀티턴 대화, 프롬프트 엔지니어링 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/1_Text_Generation/01-Text%20Generation-Lecture.ipynb) |
| [02 · Chatbot Practice ✍️](1_Text_Generation/02-Chatbot-Practice.ipynb) | 멀티턴 챗봇 클래스 직접 구현하고 `ipywidgets`로 챗봇 UI 만들기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/1_Text_Generation/02-Chatbot-Practice.ipynb) |
| [03 · Function Calling](1_Text_Generation/03-Function%20Calling-Lecture.ipynb) | Tool 정의 → Tool Call → 실행 → 결과 전달 → 최종 답변 5단계 흐름, `tool_choice` / `allowed_tools` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/1_Text_Generation/03-Function%20Calling-Lecture.ipynb) |
| [04 · Function Calling Practice ✍️](1_Text_Generation/04-Function%20Calling-Practice.ipynb) | 실시간 날씨 API(Open-Meteo) → 활동 추천으로 이어지는 Tool 체인 만들기 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/1_Text_Generation/04-Function%20Calling-Practice.ipynb) |

### Part 2. Multimodal Generation 🎨

| 노트북 | 내용 | |
| --- | --- | --- |
| [01 · Image Generation](2_Multimodal_Generation/01-Image%20Generation-Lecture.ipynb) | Responses API 이미지 생성, 투명 배경, 멀티턴 편집, 스트리밍, 레퍼런스 이미지 합성, 이미지 분석 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/2_Multimodal_Generation/01-Image%20Generation-Lecture.ipynb) |
| [02 · Video Generation 📦](2_Multimodal_Generation/02-Video%20Generation-Lecture.ipynb) | Sora 2로 영상 생성: 비동기 job → polling → 다운로드, 이미지 레퍼런스, Remix<br>⚠️ *Sora 2 / Videos API가 2026.09.24에 종료돼서 기록용(아카이브)으로 남겨뒀어요* | |
| [03 · TTS & STT](2_Multimodal_Generation/03-TTS_STT-Lecture.ipynb) | TTS(Speech API + Realtime API), STT(`gpt-transcribe`), `prompt`·`keywords`로 신조어 인식 개선, GPT 후처리 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/2_Multimodal_Generation/03-TTS_STT-Lecture.ipynb) |

### Part 3. Mini Project 🎬

| 노트북 | 내용 | |
| --- | --- | --- |
| [YouTube Summarization ✍️](3_Youtube_Summarization_Project/youtube_summarization_project.ipynb) | 유튜브 강의 오디오 → STT → Structured Output으로 요약·토픽 분리 → 토픽별 이미지 생성 → **PDF 요약본** | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/llm-api-hands-on/blob/main/3_Youtube_Summarization_Project/youtube_summarization_project.ipynb) |

<br>

## 🖼️ 이런 걸 만들어봐요

**이미지 생성 실습 결과** (고양이 & 수달, 투명 배경 스프라이트, 멀티턴 편집, 레퍼런스 합성, 로고 프린팅)

<img src="assets/image_generation_examples.jpg" width="640">

**유튜브 강의 → PDF 요약본** (3Blue1Brown의 LLM 강의를 넣어서 돌려본 결과)

<img src="assets/youtube_summary_pdf.jpg" width="640">

<details>
<summary><b>🕊️ (아카이브) 2025년에 Sora 2로 만들었던 "한강을 수영하는 비둘기"</b></summary>
<br>
<img src="assets/sora_pigeon.gif" width="200">
</details>

<br>

## 🚀 시작하기

### Colab에서 실행 (추천)

1. 위 표에서 보고 싶은 노트북의 **Open in Colab** 배지를 클릭
2. 왼쪽 사이드바 🔑 **보안 비밀**에 `OPENAI_API_KEY`를 추가하고 **노트북 액세스**를 켜기
3. 위에서부터 차례대로 실행! (실습 데이터가 필요한 노트북은 첫 셀에서 레포를 알아서 받아와요)

### 로컬에서 실행

```bash
git clone https://github.com/nawooooojin/llm-api-hands-on.git
cd llm-api-hands-on
pip install -r requirements.txt

export OPENAI_API_KEY="sk-..."   # Windows PowerShell: $env:OPENAI_API_KEY="sk-..."
jupyter lab
```

환경 변수를 안 걸어두면 노트북 실행할 때 키 입력창이 뜹니다.

> ⚠️ API 키는 노트북이나 코드에 직접 적어서 커밋하지 마세요! 깃 히스토리에 한 번 올라가면 지워도 남습니다.

### 💸 비용 안내

- OpenAI API는 사용한 만큼 과금되는 유료 서비스예요. 실습 전에 [Billing](https://platform.openai.com/settings/organization/billing)에서 크레딧을 충전해야 합니다.
- 텍스트 실습은 대부분 저렴한 `gpt-6-luna`를 써서 몇 센트 수준이고, 비용은 대부분 **이미지 생성**에서 나옵니다.
- 그래서 노트북에서는 이미지 `quality`를 `low` / `medium`으로 두었어요. 더 예쁜 결과가 필요하면 `high` 이상으로 올려보세요.

<br>

## 🔄 2026.10 업데이트 내역 (GPT-5 → 최신 API)

수업 당시(2025.11) 코드와 비교해서 바뀐 부분이에요. 예전 코드를 옮길 때 참고하세요.

| 구분 | 2025.11 수업 당시 | 2026.10 업데이트 | 비고 |
| --- | --- | --- | --- |
| 텍스트 모델 | `gpt-5` / `gpt-5-mini` / `gpt-5-nano` | `gpt-6-astra` / `gpt-6.1-sol` / `gpt-6-luna` | GPT-5 계열은 2026.12.11 종료 |
| `reasoning.effort` | `minimal` ~ `high` | `none`(luna 등) / `low` ~ `max` | `minimal` → `low`로 바꾸기 |
| 이미지 모델 | `gpt-image-1` | `gpt-image-2.5-sunburst` / `gpt-image-2.5-flare` | `input_fidelity` 미지원 |
| 비디오 | `sora-2` | — | Videos API 2026.09.24 종료 → 아카이브 |
| TTS | `gpt-4o-mini-tts` | `gpt-4o-mini-tts` + Realtime API(`gpt-realtime-2.1-mini`) | Speech API TTS 모델 2027.01.06 종료 예정 |
| STT | `gpt-4o-mini-transcribe`, `whisper-1` | `gpt-transcribe` (`languages`, `keywords`) | 기존 모델 2027.02.26 종료 예정 |
| 번역 | `audio.translations` (`whisper-1`) | 전사 → GPT 번역 2단계 | translations 엔드포인트 2027.02.26 종료 예정 |
| Prompt 객체 | `prompt={"id": "pmpt_..."}` | 프롬프트를 코드에서 직접 관리 | `v1/prompts` 2026.11.30 종료 |
| 실습 데이터 | 뉴스·상품 사진, AI Hub 음성 | `gpt-image-2.5`·TTS로 직접 생성 | 공개용으로 저작권 정리 |

> 💡 모델 이름은 진짜 빨리 바뀝니다... 실행했는데 `model not found` 같은 에러가 나면 [모델 목록](https://platform.openai.com/docs/models)에서 최신 모델명으로 바꿔서 돌려보세요!

<br>

## 📁 폴더 구조

```
llm-api-hands-on/
├── 1_Text_Generation/
│   ├── 00-OpenAI API Quick Start.ipynb
│   ├── 01-Text Generation-Lecture.ipynb
│   ├── 02-Chatbot-Practice.ipynb            ✍️
│   ├── 03-Function Calling-Lecture.ipynb
│   ├── 04-Function Calling-Practice.ipynb   ✍️
│   └── data/
├── 2_Multimodal_Generation/
│   ├── 01-Image Generation-Lecture.ipynb
│   ├── 02-Video Generation-Lecture.ipynb    📦 아카이브
│   ├── 03-TTS_STT-Lecture.ipynb
│   └── data/  (image / audio / video)
├── 3_Youtube_Summarization_Project/
│   └── youtube_summarization_project.ipynb  ✍️
├── Practice_solution/                       ✍️ 실습 정답
├── assets/                                  README용 이미지
└── requirements.txt
```

<br>

## 📝 참고 & 크레딧

- 실습 내용은 [OpenAI API 공식 문서](https://platform.openai.com/docs)와 [OpenAI Cookbook](https://cookbook.openai.com)을 바탕으로 정리했습니다.
- 실습용 이미지(`cheers.jpg`, 크리스마스 소품, 티셔츠, 캠퍼스 사진)와 음성(`data/audio/*.mp3`)은 각각 `gpt-image-2.5-sunburst`, `gpt-4o-mini-tts`로 직접 생성했어요.
- 아주대학교 로고와 마스코트 '치토'의 권리는 아주대학교에 있습니다.
- 유튜브 요약 프로젝트 예시 영상: 3Blue1Brown — [Large Language Models explained briefly](https://youtu.be/LPZh9BOjkQs) (레포에는 포함되어 있지 않고, 실행할 때 직접 받아옵니다)
- PDF 한글 폰트: [나눔고딕](https://fonts.google.com/specimen/Nanum+Gothic) (SIL Open Font License, 실행할 때 자동으로 받아옵니다)

<br>

## 📄 License

코드는 [MIT License](LICENSE)로 자유롭게 쓰셔도 됩니다. 수업 자료로 쓰실 때 출처 남겨주시면 감사하겠습니다 🙏
