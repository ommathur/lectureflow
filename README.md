# 📚 LectureFlow

**LectureFlow** is a fully automated, multimodal AI pipeline that transforms raw lecture content—videos, slide images, or transcripts—into clean, structured, human-readable notes with image-slide integration. Designed for students, researchers, and educators, LectureFlow leverages the power of LLMs, OCR, and ASR to reduce manual effort in note-taking and content summarization.

---

## 🧠 Core Idea

LectureFlow's core philosophy is that lecture content is *multimodal*. A lecture isn't just audio or slides—it's a **fusion** of both. Therefore, this system works in three stages:

1. **Understand the spoken content** via **ASR (Whisper)**.
2. **Understand the visual content** via **OCR + CLIP**.
3. **Synthesize meaningful notes** via **LLMs**.

The final result is a neatly organized `.docx` file with bullet points, sections, embedded slide images, and extracted visual content—all automatically generated.

---

## ✨ Features

- 🎥 **Transcribes Lecture Videos** using OpenAI Whisper (base/medium/large).
- 🧹 **Cleans and Segments Transcripts** into usable paragraphs.
- 🖼️ **Matches Slide Images to Content** using CLIP image-text similarity.
- 🔍 **Performs OCR** on slides to extract visible titles, keywords, and diagrams.
- ✍️ **Generates Notes with LLMs**, preserving structure and sectioning.
- 📎 **Embeds Slide Images Automatically** based on semantic relevance.
- 🗃️ **Exports Output as DOCX** (with future support for Markdown and PDF).

---

## Workflow
Video Lecture ──▶ Whisper ──▶ Transcript
                            ↓
      Slide Images ──▶ OCR & CLIP ──▶ Semantic Matching
                            ↓
        Transcript + Image Matches ──▶ LLM ──▶ .docx Notes
