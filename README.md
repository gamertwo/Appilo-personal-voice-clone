# Appilo Personal Voice Clone

## Real-Time RVC Self Voice Clone [STUPIDLY EXPLAINED]

This guide explains how to clone your own voice using **Applio + RVC** in the simplest way possible.

---

# STEP 1 — Download Applio

Download Applio from:

https://github.com/IAHispano/Applio/releases

Current size as of **27 May 2026**:

```text
~5 GB
```

Extract it and run:

```text
run-install.bat
```

After installation:

```text
run-applio.bat
```

---

# STEP 2 — Download Audacity

Download Audacity from:

https://www.audacityteam.org/download/

You will use Audacity to:

* record your voice
* split audio
* export WAV files

---

# STEP 3 — Open Applio

Applio usually opens on:

```text
http://127.0.0.1:6969/
```

or something similar like:

```text
http://localhost:6969/
```

This is NORMAL.

It opens inside your browser but runs locally on your PC.

---

# STEP 4 — Create Dataset Folder

Create a folder somewhere easy to access.

Example:

```text
dataset/myvoice
```

This folder will contain all your voice clips.

---

# STEP 5 — Record Your Voice

Open Audacity and start recording yourself speaking.

## IMPORTANT:

This is an **RVC model**, so the quality of your dataset matters A LOT.

---

# HOW TO TALK

## Best Method

Take:

* an ebook
* article
* physical book
* manga dialogue
* technical article

and read it naturally.

---

# VERY IMPORTANT RULES

Speak:

* naturally
* clearly
* medium speed
* with slight emotion
* consistent microphone distance

DO NOT:

* whisper
* scream
* act dramatically
* mumble
* rush words

---

# HOW TO SPLIT RECORDINGS

After EVERY sentence:

* pause for 1–2 seconds
* create separate clips later

Best clip size:

```text
5–15 seconds
```

NOT:

* one giant 10-minute file
* single-word clips

---

# TARGET DATASET LENGTH

Recommended:

```text
5–10 minutes total
```

Clean audio matters more than huge amounts of data.

---

# STEP 6 — Export WAV Files From Audacity

Export using these settings:

```text
WAV
Mono
16-bit PCM
32000 Hz
```

Example settings:

```text
File Type: WAV (Microsoft)
Encoding: Signed 16-bit PCM
Channels: Mono
Sample Rate: 32000 Hz
```

---

# STEP 7 — Upload Dataset Into Applio

Go to:

```text
Training → Dataset
```

Select your folder:

```text
dataset/myvoice
```

---

# STEP 8 — Training Pipeline

Inside Applio:

## 1. Preprocess Audio

Run:

```text
Preprocess
```

---

## 2. Extract Features

Use:

```text
RMVPE
```

This gives the best quality/speed balance.

---

## 3. Start Training

Recommended settings:

```text
RVC v2
32k
RMVPE
100 epochs
Batch size 8
```

---

## 4. Create Index

After training finishes:

```text
Create Index
```

This improves voice matching quality.

---

# STEP 9 — Real-Time Settings

Recommended low-latency settings:

```text
Pitch: 0
chunkSec: 4800
extraFrameSec: 960
Index Rate: 0.2
```

---

# IMPORTANT NOTES

## If voice sounds robotic:

* dataset is noisy
* clips are cut badly
* words are incomplete
* too much echo
* bad microphone

---

# BEST PRACTICES

Use:

* headphones
* quiet room
* same microphone
* consistent volume

---

# FINAL RESULT

If done correctly, you get:

* real-time voice cloning
* low latency
* lightweight model
* surprisingly accurate self voice clone

Even with:

```text
5–10 minutes
```

of clean audio.

