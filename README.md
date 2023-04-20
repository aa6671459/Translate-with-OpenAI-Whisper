# Translate-with-OpenAI-Whisper
For NHU 10924203、10924207、10924308 AI Midterm
# 將.ipynb檔案跟想要進行語音轉文字辨識的檔案放入google colab，修改檔案來源即可使用
# 此內容皆從網路上擷取，用來學習之使用

-
安裝whisper、ffmpng套件
<br>
  !pip install git+https://github.com/openai/whisper.git
  !sudo apt update && sudo apt install ffmpeg
-
掛載雲端硬碟
<br>
  from google.colab import drive
<br>
  drive.mount('/content/drive')
<br>
-
辨識音檔
<br>
  !whisper "要辨識的音檔" --model medium
-
翻譯音檔之後再進行文字檔輸出
<br>
  !whisper "要辨識的音檔" --task translate
-
