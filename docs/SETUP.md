# 📖 Detailed Setup & Configuration Guide

## Table of Contents
- [Getting Your API Key](#-getting-your-api-key)
- [Local Setup](#-local-setup)
- [Deployment](#-deployment)
- [Troubleshooting](#-troubleshooting)
- [FAQ](#-faq)

---

## 🔑 Getting Your API Key

### Step 1: Visit Google AI Studio
Open your browser and go to: **https://makersuite.google.com/app/apikey**

### Step 2: Sign In
- Sign in with your Google account
- If you don't have one, create a free Google account (takes 2 minutes)

### Step 3: Create API Key
1. Click the blue **"Create API Key"** button
2. Select **"Create API key in new project"**
3. Your API key will be generated and displayed
4. Click **"Copy"** to copy it to clipboard

### Step 4: Use in App
1. Open `index.html` in your browser
2. A popup will ask for your API key
3. Paste your copied API key
4. Click **"Set API Key"**
5. Done! The app will verify your key and you're ready to translate

---

## 💻 Local Setup

### Option A: Using GitHub Desktop (Easiest)
1. Download [GitHub Desktop](https://desktop.github.com/)
2. Click **"File"** → **"Clone Repository"**
3. Paste: `https://github.com/yourusername/real-time-language-translator`
4. Choose where to save
5. Open the folder and double-click `index.html`

### Option B: Using Command Line
```bash
# Open Terminal/Command Prompt

# Clone the repository
git clone https://github.com/yourusername/real-time-language-translator.git

# Navigate to folder
cd real-time-language-translator

# Open in browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

### Option C: Direct Download (No Git Needed)
1. Go to the GitHub repository
2. Click **"Code"** → **"Download ZIP"**
3. Extract the ZIP file
4. Double-click `index.html` to open in browser

---

## 🌐 Deployment

### Deploy to GitHub Pages (Free Hosting)

**Prerequisites:** GitHub account (free)

**Steps:**

1. **Go to Your Repository**
   - Navigate to your GitHub repository
   - Click **"Settings"**

2. **Enable GitHub Pages**
   - Scroll to **"GitHub Pages"** section
   - Select **"Deploy from a branch"**
   - Branch: **"main"**
   - Folder: **"/ (root)"**
   - Click **"Save"**

3. **Wait for Deployment**
   - GitHub will build and deploy your site
   - Takes about 2-5 minutes
   - You'll see a green checkmark when ready

4. **Access Your Live Site**
   - Your site will be available at:
   ```
   https://yourusername.github.io/real-time-language-translator/
   ```

5. **Share Your Link**
   - Add this to your resume/portfolio
   - Share on LinkedIn
   - Send to potential employers

---

## 🛠️ Troubleshooting

### Issue: "Microphone access denied"

**Solution:**
1. **Chrome/Edge:**
   - Click the lock icon next to URL
   - Find "Microphone"
   - Click "Allow"
   - Refresh the page

2. **Firefox:**
   - Click the lock icon next to URL
   - Click arrow next to "Microphone"
   - Select "Allow"

3. **Safari:**
   - System Preferences → Security & Privacy → Microphone
   - Find Safari and check if it's allowed

---

### Issue: "API Key not working"

**Checklist:**
- [ ] Did you copy the entire key? (Very long string)
- [ ] Is your internet connection working?
- [ ] Are you using the latest browser version?
- [ ] Did you try in a different browser?

**Solution:**
1. Go back to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Check if your API key is still there
3. If missing, create a new one
4. Clear browser cache:
   - **Chrome:** Settings → Privacy → Clear browsing data
   - **Firefox:** Preferences → Privacy → Clear Data
5. Try again

---

### Issue: "Translation takes too long"

**Normal behavior:**
- First translation: 1-3 seconds (API startup)
- Subsequent translations: 1-2 seconds
- Depends on internet speed

**If consistently slow:**
1. Check your internet speed (need at least 1 Mbps)
2. Try a different language pair
3. Try in a different browser

---

### Issue: "No audio output"

**Troubleshooting steps:**

1. **Check Volume:**
   - Is your computer volume on?
   - Is the browser tab muted? (Click unmute icon)

2. **Check Browser Settings:**
   - Chrome: Settings → Privacy → Permissions → Audio
   - Firefox: Preferences → Privacy → Audio
   - Make sure app is allowed

3. **Try Speaker Button:**
   - Click the speaker icon in output area
   - Listen with headphones

4. **Language Support:**
   - Some languages may use browser TTS (slightly different voice)
   - This is normal, audio will still work

---

### Issue: "Browser showing blank page"

**Solution:**
1. **Check if JavaScript is enabled:**
   - Chrome: Settings → Privacy → JavaScript → Allowed
   - Firefox: about:config → javascript.enabled → true

2. **Try different browser:** Chrome, Firefox, or Safari

3. **Check browser console for errors:**
   - Press F12 to open Developer Tools
   - Look at "Console" tab
   - Share any error messages for help

---

### Issue: "Gemini-2.5-flash-preview-tts not found"

This is a known issue with newer Gemini models. The app automatically falls back to browser text-to-speech, which works perfectly fine. No action needed - just keep using the app!

---

## ❓ FAQ

### Q: Is this free to use?
**A:** Yes! The app and Google Gemini API are both free for standard usage.

### Q: Will you see my API key?
**A:** No. Your API key is stored only in your browser's local storage. It's never sent to anyone except Google's official API servers.

### Q: What if I share my computer?
**A:** The API key is saved locally. If you share a computer, consider clearing browser data before sharing. Or create a project-specific API key in Google AI Studio.

### Q: Does the app work offline?
**A:** No, you need an internet connection for translation. The speech recognition works locally, but translation requires API calls.

### Q: Can I use this commercially?
**A:** Yes! The app is MIT licensed. You can use it for personal or commercial projects.

### Q: How many translations can I do?
**A:** Google's free tier is very generous - typically 15,000 requests per minute. You won't hit these limits unless you're using it at massive scale.

### Q: What languages are supported?
**A:** 100+ languages including all major world languages. The exact list depends on Google Gemini's supported languages.

### Q: Can I modify the code?
**A:** Yes! The code is intentionally simple and well-commented. Feel free to customize colors, fonts, languages, etc.

### Q: How do I customize the app?

**Change Colors:**
```css
/* In index.html, find and modify: */
background: #5e1f04;  /* Primary color */
```

**Add More Languages:**
```html
<option value="language-code">Language Name</option>
```

**Change Font:**
```css
body {
    font-family: "Arial", sans-serif;  /* Change from Poppins */
}
```

### Q: Can I add this to my portfolio?
**A:** Absolutely! This is perfect for showing:
- JavaScript skills
- API integration
- Web design
- User experience thinking
- Problem-solving abilities

---

## 📞 Getting Help

### Where to Find Help

1. **In-App Issues:**
   - Check the console (F12 → Console tab)
   - Status messages will tell you what's wrong

2. **GitHub:**
   - Create an issue on the repository
   - Include: what you were doing, what went wrong, your browser

3. **Google API Issues:**
   - Check [Google AI Documentation](https://ai.google.dev/docs)
   - Verify your API key is valid

4. **Web Speech API Issues:**
   - Not all browsers support speech recognition
   - Chrome and Firefox have the best support

---

## 📚 Learning Resources

### JavaScript Concepts Used
- **Fetch API** - Making HTTP requests
- **Web Speech API** - Speech recognition
- **Local Storage** - Saving data in browser
- **Async/Await** - Handling asynchronous operations
- **DOM Manipulation** - Updating HTML elements

### Useful Links
- [MDN Web APIs](https://developer.mozilla.org/en-US/docs/Web/API)
- [Google Generative AI Docs](https://ai.google.dev/)
- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)
- [Fetch API Guide](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

---

## 🚀 Next Steps

1. ✅ Set up your API key
2. ✅ Test the app locally
3. ✅ Deploy to GitHub Pages
4. ✅ Add to your portfolio/resume
5. ✅ Share on LinkedIn/GitHub
6. ✅ Consider enhancements (dark mode, history, etc.)

---

**Happy Translating!** 🌍✨
