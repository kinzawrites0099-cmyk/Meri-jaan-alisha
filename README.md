readme = '''# 🎂 Happy Birthday Meri Jaan Alisha 🎂

A beautiful birthday website for Alisha made with love by Rohaan!

## 📁 Files Structure

```
alisha-birthday/
├── index.html      # Page 1: Happy Birthday Meri Jaan Alisha
├── song.html       # Page 2: Music & Games
├── reply.html      # Page 3: Reply to her letters
├── poetry.html     # Page 4: Poetry for Alisha
└── images/         # Folder containing letter images
    ├── letter1.jpg
    ├── letter2.jpg
    ├── letter3.jpg
    ├── letter4.jpg
    ├── letter5.jpg
    ├── letter6.jpg
    └── letter7.jpg
```

## 🚀 How to Upload on GitHub

### Step 1: Create GitHub Account
1. Go to [github.com](https://github.com)
2. Sign up for free

### Step 2: Create New Repository
1. Click on "+" icon (top right)
2. Select "New repository"
3. Name it: `alisha-birthday`
4. Make it Public
5. Click "Create repository"

### Step 3: Upload Files
1. Click "uploading an existing file"
2. Drag and drop all files (index.html, song.html, reply.html, poetry.html)
3. Create folder named `images` and upload all letter images there
4. Click "Commit changes"

### Step 4: Enable GitHub Pages
1. Go to repository "Settings"
2. Click "Pages" (left sidebar)
3. Under "Source", select "main" branch
4. Click "Save"
5. Wait 2-3 minutes
6. Your site will be live at: `https://yourusername.github.io/alisha-birthday/`

## 🎵 Adding Birthday Song

1. Download "Happy Birthday" MP3 song
2. Rename it to `happy-birthday.mp3`
3. Upload it in the same folder as HTML files
4. Update the audio source in `song.html`

## 💝 Features

- ✨ Beautiful animations
- 🎵 Background music
- 🎮 Interactive games
- 📜 Letter gallery with lightbox
- 🌹 Romantic poetry
- 📱 Mobile responsive

## 💌 Made with Love

For: Alisha ❤️
From: Rohaan

---

*"Tum meri life ka sabse khubsurat hissa ho"*
'''

with open('/mnt/agents/output/alisha-birthday/README.md', 'w', encoding='utf-8') as f:
    f.write(readme)

print("README.md created!")

# List all files
import os
print("\n📁 Files in output folder:")
for root, dirs, files in os.walk('/mnt/agents/output/alisha-birthday'):
    level = root.replace('/mnt/agents/output/alisha-birthday', '').count(os.sep)
    indent = ' ' * 2 * level
    print(f'{indent}{os.path.basename(root)}/')
    subindent = ' ' * 2 * (level + 1)
    for file in files:
        print(f'{subindent}{file}')
