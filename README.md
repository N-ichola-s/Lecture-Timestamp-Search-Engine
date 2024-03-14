WORK IN PROGRESS (this is my senior capstone this semester, will update as we go):

Lecture Search Engine

Goal: build a search engine for explanations or definitions of technical concepts that are explained in videos

Possible data: lectures on YouTube

Possible approach:

A. Identify a list of lectures on YouTube, and either save them or save their video IDs.

B. Obtain the subtitles for them. Either use their API or download the audios (e.g., with youtube-dl) and compute their subtitles (e.g., with Whisper).

C. Build a search engine from the subtitles. When a user makes a query, display the correct moment from a video.

Possible evaluation: annotate some data as gold standard and use standard information retrieval metrics but also accounting for the moment within the video

Youtube transcriptions data set:

https://huggingface.co/datasets/jamescalam/youtube-transcriptions/blob/main/README.md
