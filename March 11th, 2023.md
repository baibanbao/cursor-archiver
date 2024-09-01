- [https://writing.upenn.edu/library/Mayer-Bernadette\_Experiments.html?utm\_source=substack&utm\_medium=email](https://writing.upenn.edu/library/Mayer-Bernadette_Experiments.html?utm_source=substack&utm_medium=email)
- [自定义知识库聊天机器人.ipynb - Colaboratory](https://colab.research.google.com/drive/1Fr1hxYOG5lss9vbvZlaw-11wM2U6N7cQ)
- whisper
    - [ggerganov/whisper.cpp: Port of OpenAI's Whisper model in C/C++](https://github.com/ggerganov/whisper.cpp)
    - [blog/2023-03-01：whisper.cpp 語音轉文字教學.md at master · flameddd/blog](https://github.com/flameddd/blog/blob/master/2023-03-01%EF%BC%9Awhisper.cpp%20%E8%AA%9E%E9%9F%B3%E8%BD%89%E6%96%87%E5%AD%97%E6%95%99%E5%AD%B8.md)
    - 我的第一个编程
        - ```python
# Import the OpenAI library
import openai

# Set the OpenAI API key
openai.api_key = "这里换成你自己的API"

# Open the audio file in binary mode
with open("/Users/ding/Downloads/gpt-coding/huxueyan-01.mp3", "rb") as audio_file:
    # Transcribe the audio file using the OpenAI API
    transcript = openai.Audio.transcribe("whisper-1", audio_file, prompt="这是王刚播讲的《红顶商人胡雪岩》", response_format="srt")
    
    # Write the transcription to a file
    with open("transcript-3.srt", "w") as f:
        f.write(transcript)```
    -  又编了一个纯文本输出的
        - ```python
# Import the OpenAI library
import openai

# Set the OpenAI API key
openai.api_key = "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"

# Open the audio file in binary mode
with open("/Users/ding/Downloads/gpt-coding/20230129-short-sermon.mp3", "rb") as audio_file:
    # Transcribe the audio file using the OpenAI API
    transcript = openai.Audio.transcribe("whisper-1", audio_file, prompt="这是下午短讲的内容", response_format="text")
    
    # Write the transcription to a file
    with open("20230129-short-sermon.txt", "w") as f:
        f.write(transcript)```
- 整理文本
    - 直接用[[ChatGPT]]，让它加标点，分段落，这个它最擅长了
- 今天开心的事
    - 解决了[[drafts]]的action问题
        - 原来需要先forget 秘密
            - [Credentials | Drafts User Guide](https://docs.getdrafts.com/docs/settings/credentials#forgetting-credentials-logout)
        - 然后再打开ChatGPT Conversation Action就可以工作如初了
