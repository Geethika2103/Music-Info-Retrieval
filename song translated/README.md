
### Step 1: install Whisper with pip

```bash
pip install git+https://github.com/openai/whisper.git
```

---

### 🔧 Step 2: install `ffmpeg` (required for audio processing)

```bash
sudo apt install ffmpeg
```

---

### Step 3: Created and activated a Conda environment



```bash
conda create -n whisper_env python=3.9 -y
conda activate whisper_env
```

---

### 📂 Step 4: Run  Whisper from your Downloads directory

You navigated to the folder:

```bash
cd ~/Downloads
```

And run the transcription command:

```bash
whisper "yodha padakali tamil.mp3" --language ta --model medium --fp16 False
```
for malayalam 

```bash
whisper "your_malayalam_audio.mp3" --language ml --model medium --fp16 False

```

### CHATGPT PROMPT

*Give the list of movies which are dubbed from malayalam to tamil ,vice versa

*Take a movie and ask: Give the list of songs from this movie(movie name in malayalam and tamil) which is having exact line by line translation of the song from malayalam to tamil  or vice versa

*| Song Title                           | Malayalam → Tamil Translation | Meaning Fidelity             |
| ------------------------------------ | ----------------------------- | ---------------------------- |
| **Jeeva Nadhi**                      | ஜீவ நதி                       | 🔁 Exact line-by-line        |
| **Deerane**                          | தீரனே                         | 🔁 Exact line-by-line        |
| **Siva Sivaya Potri**                | —                             | 🔁 Exact devotional lyrics   |
| *Manohari, Irul Konda Vaanil*        | —                             | ✂️ Poetic adaptations        |
| *Kanna Nee Urangada* (*Baahubali 2*) | —                             | 🎤 Very faithful translation |

### *For malayalam lyrics use:

```bash

https://m3db.com/lyric/35179

```

### For tamil lyrics:

Use whisper which was installed lately or use:

```bash

https://tamilpadalvarigal.com/kanna-nee-thoongadaa-song-lyrics-in-tamil/

```
*After getting  the lyrics copy paste the lyrics ask chatgpt to : remove unwanted writings like male ,female and just give the complete lyrics

### * To check whether both malayalam and tamil song is having same meaning use:

```bash
https://translate.google.co.in/?sl=en&tl=de&op=translate

```

