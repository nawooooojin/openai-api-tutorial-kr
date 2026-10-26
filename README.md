# 🤖 OpenAI API Hands-on

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-GPT--6-412991?logo=openai&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-ready-F9AB00?logo=googlecolab&logoColor=white)
![Last Updated](https://img.shields.io/badge/updated-2026.10-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

아주대학교 「모바일컴퓨팅특론」 수업에서 진행했던 OpenAI API 실습 자료입니다.

텍스트 생성부터 Function Calling, 이미지·음성 생성까지 다루고, 마지막에는 유튜브 강의를 PDF 요약본으로 만드는 프로젝트로 마무리합니다.
2026년 10월 기준 API(GPT-6, gpt-image-2.5, gpt-transcribe 등)로 작성되어 있으며, Colab에서 바로 실행할 수 있습니다.

<br>

## 📚 Curriculum

✍️ 표시는 `TODO` 빈칸을 채우는 실습 노트북이며, 정답은 [`Practice_solution/`](Practice_solution/)에 있습니다.

### Part 1. Text Generation

Responses API 기본 사용법부터 멀티턴 대화, 프롬프트 작성, Function Calling까지 다룹니다.

| 노트북 | 내용 | |
| --- | --- | --- |
| [00 · OpenAI API Quick Start](1_Text_Generation/00-OpenAI%20API%20Quick%20Start.ipynb) | Responses API 기본 호출, 이미지 입력, 웹 검색, 스트리밍 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/1_Text_Generation/00-OpenAI%20API%20Quick%20Start.ipynb) |
| [01 · Text Generation](1_Text_Generation/01-Text%20Generation-Lecture.ipynb) | 주요 파라미터, 모델 비교, `reasoning.effort` / `text.verbosity`, 멀티턴 대화, 프롬프트 엔지니어링 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/1_Text_Generation/01-Text%20Generation-Lecture.ipynb) |
| [02 · Chatbot Practice ✍️](1_Text_Generation/02-Chatbot-Practice.ipynb) | 멀티턴 챗봇 클래스 구현, `ipywidgets` 챗봇 UI | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/1_Text_Generation/02-Chatbot-Practice.ipynb) |
| [03 · Function Calling](1_Text_Generation/03-Function%20Calling-Lecture.ipynb) | Tool 정의 → 호출 → 결과 전달 흐름, `tool_choice` / `allowed_tools` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/1_Text_Generation/03-Function%20Calling-Lecture.ipynb) |
| [04 · Function Calling Practice ✍️](1_Text_Generation/04-Function%20Calling-Practice.ipynb) | 실시간 날씨 API(Open-Meteo) → 활동 추천으로 이어지는 Tool 체인 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/1_Text_Generation/04-Function%20Calling-Practice.ipynb) |

### Part 2. Multimodal Generation

이미지 생성·편집·분석과 TTS/STT를 다룹니다. Video Generation은 Sora 2 API 종료(2026.09)로 수업 당시의 실행 결과만 남겨두었습니다.

| 노트북 | 내용 | |
| --- | --- | --- |
| [01 · Image Generation](2_Multimodal_Generation/01-Image%20Generation-Lecture.ipynb) | 이미지 생성, 투명 배경, 멀티턴 편집, 스트리밍, 레퍼런스 이미지 편집, 이미지 분석 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/2_Multimodal_Generation/01-Image%20Generation-Lecture.ipynb) |
| [02 · Video Generation](2_Multimodal_Generation/02-Video%20Generation-Lecture.ipynb) | Sora 2 비동기 job 생성 → polling → 다운로드, 이미지 레퍼런스, Remix (아카이브) | |
| [03 · TTS & STT](2_Multimodal_Generation/03-TTS_STT-Lecture.ipynb) | Speech API / Realtime API로 음성 생성, `gpt-transcribe` 전사, prompt·keywords로 신조어 인식 개선, GPT 후처리 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/2_Multimodal_Generation/03-TTS_STT-Lecture.ipynb) |

### Part 3. Project

STT, Structured Output, 이미지 생성을 하나로 엮어 유튜브 강의를 PDF 요약본으로 만드는 프로젝트입니다.

| 노트북 | 내용 | |
| --- | --- | --- |
| [YouTube Summarization ✍️](3_Youtube_Summarization_Project/youtube_summarization_project.ipynb) | 유튜브 오디오 추출 → STT → 요약·토픽 분리 → 토픽별 이미지 생성 → PDF 요약본 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nawooooojin/openai-api-hands-on/blob/main/3_Youtube_Summarization_Project/youtube_summarization_project.ipynb) |

<br>

## 🖼️ Examples

**Image Generation**

<img src="assets/image_generation_examples.jpg" width="640">

**YouTube Summarization** — 3Blue1Brown의 LLM 강의로 만든 PDF 요약본

<img src="assets/youtube_summary_pdf.jpg" width="640">

<details>
<summary><b>Video Generation (2025, Sora 2)</b></summary>
<br>
<img src="assets/sora_pigeon.gif" width="200">
</details>

<br>

## 🚀 Getting Started

OpenAI API 키가 필요합니다. ([API 키 발급](https://platform.openai.com/api-keys))

### Colab

1. 위 표에서 노트북의 **Open in Colab** 배지를 클릭합니다.
2. 왼쪽 사이드바 🔑 **보안 비밀**에 `OPENAI_API_KEY`를 추가하고 노트북 액세스를 허용합니다.
3. 위에서부터 순서대로 실행합니다. 실습 데이터는 첫 셀에서 자동으로 받아옵니다.

### Local

```bash
git clone https://github.com/nawooooojin/openai-api-hands-on.git
cd openai-api-hands-on
pip install -r requirements.txt

export OPENAI_API_KEY="sk-..."   # Windows PowerShell: $env:OPENAI_API_KEY="sk-..."
jupyter lab
```

<br>

## 📁 Structure

```
openai-api-hands-on/
├── 1_Text_Generation/
│   ├── 00-OpenAI API Quick Start.ipynb
│   ├── 01-Text Generation-Lecture.ipynb
│   ├── 02-Chatbot-Practice.ipynb
│   ├── 03-Function Calling-Lecture.ipynb
│   ├── 04-Function Calling-Practice.ipynb
│   └── data/
├── 2_Multimodal_Generation/
│   ├── 01-Image Generation-Lecture.ipynb
│   ├── 02-Video Generation-Lecture.ipynb
│   ├── 03-TTS_STT-Lecture.ipynb
│   └── data/
├── 3_Youtube_Summarization_Project/
│   └── youtube_summarization_project.ipynb
├── Practice_solution/
├── assets/
└── requirements.txt
```

<br>

## 📄 License

MIT License
