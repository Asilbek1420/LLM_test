# LLM_test
For transcript and translation testing

Do downloading and transcription on the backend.

Let the app do the translation using OpenAI/DeepSeek directly via API calls.

This splits the workload and may reduce server costs.

- You paste a YouTube link (or type it in)

- You press a button

>>> The app downloads → transcribes → translates

>>> All results appear automatically


**
Example simple flow with REST API**
Server A downloads audio, uploads it to Server B’s /upload_audio endpoint

Server B saves audio, processes transcription, then calls Server C’s /translate endpoint with transcription text

Server C returns translation result to Server B or user-facing app
