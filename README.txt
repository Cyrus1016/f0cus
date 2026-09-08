FOCUS  -  install instructions

This is a Progressive Web App. It runs from a normal web address and installs like a native app on Windows, Mac, iPhone, and Android. Data is stored on each device.

1. HOST THE FOLDER
   The files need to be served over https (or http://localhost). Easiest options:
   a) GitHub Pages: create a repo, upload these files, enable Pages in Settings. You get https://yourname.github.io/repo/
   b) Netlify Drop: drag this folder onto https://app.netlify.com/drop
   c) Local on your PC: open a terminal in this folder and run   python -m http.server 8080   then visit http://localhost:8080

2. INSTALL ON WINDOWS (Chrome or Edge)
   Open the address, click the install icon at the right end of the address bar (or menu > "Install Focus"). It becomes a standalone window you can pin to the taskbar and snap into a FancyZone.
   To auto-launch at startup, put a shortcut to the installed app in shell:startup, or use
   start chrome --app=https://YOUR-URL   in your startup batch file.

3. INSTALL ON IPHONE (Safari)
   Open the address in Safari, tap Share, tap "Add to Home Screen". It opens full screen with no browser chrome.

4. INSTALL ON MAC
   Chrome or Edge: same install button as Windows. Safari: File > Add to Dock.

NOTES
- Notifications and the transition sounds need the app to have been interacted with once (press play).
- Data lives in the browser storage of the device that installed it. Use Export CSV in Statistics to move it.
- Opening index.html directly as a file also works for the timer, but the install button and offline cache require it to be served (step 1).
