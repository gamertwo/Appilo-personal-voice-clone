Appilo Personal Voice Clone
Real-Time RVC Self Voice Clone [STUPIDLY EXPLAINED]

This guide explains how to clone your own voice using Applio + RVC in the simplest way possible.

STEP 1 — Download Applio

Download Applio from:

Applio GitHub Releases

Current size as of 27 May 2026:

~5 GB

Extract it and run:

run-install.bat

After installation:

run-applio.bat
STEP 2 — Download Audacity

Download Audacity from:

Audacity Official Website

You will use Audacity to:

record your voice
split audio
export WAV files
STEP 3 — Open Applio

Applio usually opens on:

http://127.0.0.1:6969/

or something similar like:

http://localhost:6969/

This is NORMAL.

It opens inside your browser but runs locally on your PC.

STEP 4 — Create Dataset Folder

Create a folder somewhere easy to access.

Example:

dataset/myvoice

This folder will contain all your voice clips.

STEP 5 — Record Your Voice

Open Audacity and start recording yourself speaking.

IMPORTANT:

This is an RVC model, so the quality of your dataset matters A LOT.

HOW TO TALK
Best Method

Take:

an ebook
article
physical book
manga dialogue
technical article

and read it naturally.

VERY IMPORTANT RULES

Speak:

naturally
clearly
medium speed
with slight emotion
consistent microphone distance

DO NOT:

whisper
scream
act dramatically
mumble
rush words
HOW TO SPLIT RECORDINGS

After EVERY sentence:

pause for 1–2 seconds
create separate clips later

Best clip size:

5–15 seconds

NOT:

one giant 10-minute file
single-word clips
TARGET DATASET LENGTH

Recommended:

5–10 minutes total

Clean audio matters more than huge amounts of data.

STEP 6 — Export WAV Files From Audacity

Export using these settings:

WAV
Mono
16-bit PCM
32000 Hz

Example settings:

<img width="612" height="398" alt="image" src="https://github.com/user-attachments/assets/4ae6a4bc-6411-402c-9762-0778b72d6a02" />
STEP 7 — Upload Dataset Into Applio

Go to:

Training → Dataset

Select your folder:

dataset/myvoice
STEP 8 — Training Pipeline

Inside Applio:

1. Preprocess Audio

Run:

Preprocess
2. Extract Features

Use:

RMVPE

This gives the best quality/speed balance.

3. Start Training

Recommended settings:

RVC v2
32k
RMVPE
100 epochs
Batch size 8
4. Create Index

After training finishes:

Create Index

This improves voice matching quality.

STEP 9 — Real-Time Settings

Recommended low-latency settings:

Pitch: 0
chunkSec: 4800
extraFrameSec: 960
Index Rate: 0.2
