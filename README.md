# Social Preview for After Effects

A panel that previews your comp under the **Instagram Reels**, **Instagram
Story** and **TikTok** interface, so you can check that text and key moments
clear the app's buttons, captions and safe zones before you deliver.

The overlays go on top of your comp as locked adjustment layers, set as guide
layers so they never show up in your renders.

## Install

Close After Effects first.

**Mac** (the same command installs and updates):

```bash
curl -fsSL https://github.com/djkim-wbd/ae-social-preview-dist/releases/latest/download/install | bash
```

**Windows** (PowerShell):

```powershell
irm https://github.com/djkim-wbd/ae-social-preview-dist/releases/latest/download/install.ps1 | iex
```

### Prefer not to use the Terminal?

1. Open the [latest release](https://github.com/djkim-wbd/ae-social-preview-dist/releases/latest).
2. Download **Social-Preview.zip** and unzip it.
3. Double-click **Install Social Preview** (Mac) or **Install Social Preview.bat** (Windows).
4. If your Mac says it can't be opened, right-click it, choose **Open**, then **Open** again.

## Use it

1. Open After Effects and choose **Window → Extensions → Social Preview**.
2. Open the comp you want to check (it's designed for 9:16, 1080×1920).
3. Click **Instagram Reels**, **Instagram Story** or **TikTok**. Click **Off** to hide them.
4. Turn on the guides you need (safe zone, 4:5 feed crop, 3:4 profile grid) and
   type your own username and caption to see how they wrap.

The UI only appears where your comp has pixels. Over empty (transparent) parts
of the frame there is nothing for the overlay to sit on.

## Updates

- **Platform layouts update by themselves.** When Instagram or TikTok change
  their app, the panel downloads the new layouts the next time it opens. If an
  overlay in your comp is out of date, the panel offers a **Rebuild** button.
- **New versions of the panel** show a **Get update** button in the panel. Run
  the install command above again, or download the new zip.

## Uninstall

Delete the folder `com.socialpreview.aftereffects` from:

- **Mac:** `~/Library/Application Support/Adobe/CEP/extensions/`
- **Windows:** `%APPDATA%\Adobe\CEP\extensions\`

Then restart After Effects.
