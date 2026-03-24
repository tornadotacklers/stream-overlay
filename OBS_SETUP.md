# Adding the Overlay to OBS — Step by Step

## Requirements
- OBS Studio (any recent version)
- Your overlay hosted on GitHub Pages (see README.md)

---

## Step 1 — Copy Your GitHub Pages URL

After enabling GitHub Pages, your URL will look like:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/stream_layout.html
```
Copy this URL — you'll need it in Step 3.

---

## Step 2 — Add a Browser Source in OBS

1. Open **OBS Studio**
2. In the **Sources** panel at the bottom, click the **+** button
3. Select **Browser**
4. Name it something like `Storm Overlay` and click **OK**

---

## Step 3 — Configure the Browser Source

Fill in the settings exactly as follows:

| Setting | Value |
|---|---|
| **URL** | Your GitHub Pages URL from Step 1 |
| **Width** | `1920` |
| **Height** | `1080` |
| **Use custom frame rate** | Unchecked |
| **Control audio via OBS** | Unchecked |
| **Shutdown source when not visible** | ❌ Unchecked |
| **Refresh browser when scene becomes active** | ✅ Checked |

Scroll down and **clear out any Custom CSS** — leave that box empty.

Click **OK**.

---

## Step 4 — Allow Location Permission

1. Right-click the Browser source in your Sources panel
2. Click **Interact**
3. A small browser window will pop up — click **Allow** when it asks for your location
4. OBS will remember this permission going forward

---

## Step 5 — Position the Overlay

1. In OBS, right-click the Browser source
2. Click **Transform → Fit to Screen**
3. The overlay will fill your canvas — the top bar sits at the very top, everything else is transparent

---

## Troubleshooting

**Location shows "LOCATING..." and never updates**
→ Go back to Step 4 and make sure you clicked Allow in the Interact window

**Top bar not visible**
→ Make sure Width is 1920 and Height is 1080 in the browser source settings

**Temperature shows --°F**
→ Location permission may be blocked. Re-do Step 4.

**Tornado warning not triggering**
→ NWS alerts only fire for active Tornado Warnings (not watches). This is working correctly if no warning is issued for your area.

---

*For support contact: startekno@gmail.com*
