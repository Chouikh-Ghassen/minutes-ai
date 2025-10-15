# Minutes AI 🧠🎙️

AI-powered meeting minutes generator built with **Whisper** and **LLaMA 3**.  
Upload or record meeting audio, and get clean, structured minutes with summaries, discussion points, and action items.

---

## 🚀 Run it in Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Chouikh-Ghassen/minutes-ai/blob/main/minutes_ai.ipynb)

---

## 🧩 Tech Stack
- **Whisper** → automatic speech-to-text transcription  
- **LLaMA 3** → summarization and minute generation  
- **Gradio** → interactive web UI  

---

## 🗂️ Dataset Source

This project uses a real meeting sample from the  
[MeetingBank dataset](https://huggingface.co/datasets/huuuyeah/MeetingBank_Audio) — a benchmark collection of U.S. city-council meetings with transcripts and summaries.

Since the full dataset is very large (over **3,500 hours** of meetings), we provide **one example audio file** that can be used for testing the model without downloading the entire dataset.

To make testing easier, a copy of this example audio file is included in this repository.  
[Audio_file: denver_meeting_file.mp3](https://drive.google.com/file/d/1-R5EBNuebkcH_3gbTJXLpoqN30ZcGt95/view?usp=sharing)
After downloading, upload it to your Google Drive and reference it in Colab:

```python
from google.colab import drive
drive.mount('/content/drive')
audio_filename = "/content/drive/MyDrive/denver_meeting_file.mp3"
```

## 🧾 Dataset Acknowledgement

This project uses data from the [MeetingBank dataset](https://huggingface.co/datasets/huuuyeah/meetingbank),  
created by **Yebowen Hu, Tim Ganter, Hanieh Deilamsalehy, Franck Dernoncourt, Hassan Foroosh, and Fei Liu**,  
and presented in the paper:

> **MeetingBank: A Benchmark Dataset for Meeting Summarization**  
> *Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (ACL 2023), Toronto, Canada.*


```bibtex
@inproceedings{hu-etal-2023-meetingbank,
    title = "MeetingBank: A Benchmark Dataset for Meeting Summarization",
    author = "Yebowen Hu and Tim Ganter and Hanieh Deilamsalehy and Franck Dernoncourt and Hassan Foroosh and Fei Liu",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (ACL)",
    month = July,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics"
}
```





MIT License © 2025 [Chouikh Ghassen](https://github.com/Chouikh-Ghassen)
