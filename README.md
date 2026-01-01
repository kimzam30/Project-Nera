# 📟 Terminal-Style Animated Letter (Template)

A web-based, interactive personal letter styled like a retro command-line interface (CLI). This project is designed as a **template** for creating a sentimental or romantic surprise.

It features a typewriter text effect, background audio, and a cinematic image reveal.

## ✨ Features

- **Retro Aesthetic:** "Hacker Green" terminal text on a dark background.
- **Immersive Audio:** Background music fades in upon initialization.
- **Typewriter Effect:** JavaScript-driven text rendering mimicking real-time typing.
- **Dynamic Reveal:** Two-stage message delivery followed by an image and heartbeat animation.
- **Privacy Focused:** Media files are excluded by default so you can safely customize it.

## 📂 Project Structure

```text
/project-root
│
├── index.html       # Main application file
├── .gitignore       # Excludes specific media files (song.mp3, us.jpg)
└── README.md        # Documentation
Note: The song.mp3 and us.jpg files are listed in .gitignore to prevent accidental upload of sensitive media to public repositories.
```

## 🚀 How to Use (Local Setup)

### **Since this is a template, you must add your own media assets before running it.**

### Clone the repository:

```
Bash
git clone [https://github.com/yourusername/your-repo-name.git](https://github.com/yourusername/your-repo-name.git)
```

- Add your assets:
- Find a song you like and rename it to song.mp3.
- Find a photo you want to reveal and rename it to us.jpg.
- Move both files into the root folder of the project.
- Open index.html in your browser to test.

## 🛠️ Configuration

### To customize the text, open index.html in your code editor.

- Edit the Conversation: Locate the myInsecurities and myReasons arrays near line 115 in the JavaScript section.
- Edit the Final Message: Locate finalP.innerHTML near line 182.
- Adjust Timing: You can tweak the delay values in the runSequence() function to match the tempo of your song.

## ☁️ Deployment (Netlify Manual Drop)

### **Because this repository excludes the media files, you cannot use Netlify's "Import from GitHub" feature directly, or your site will launch without music or images.**

### Follow these steps to deploy your full version:

- Prepare your Local Folder: Ensure your local project folder contains index.html, song.mp3, and us.jpg.
- Log in to Netlify: Go to Netlify.com and log in.
- Navigate to Sites: Go to the "Sites" tab in your dashboard.
- Drag & Drop: Drag your entire project folder from your computer and drop it into the box that says "Drag and drop your site output folder here".
- Done! Netlify will upload your assets and give you a live URL instantly.

#

### **_This project is open source and available for personal use._**
