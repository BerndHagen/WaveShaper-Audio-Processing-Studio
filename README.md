<p align="center">
  <img src="images/waveshaper-logo.png" alt="WaveShaper Logo" width="128" />
</p>
<h1 align="center">WaveShaper - Audio Processing Studio</h1>
<p align="center">
  <b>Shape your sound with professional-grade audio processing, EQ mastering and real-time visualization.</b><br>
  <b>Experience a powerful, intuitive audio workstation optimized for precision and performance.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/WaveShaper-Audio-Processing-Studio?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freemium-red?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**WaveShaper** is a professional audio processing application designed for musicians, producers and audio enthusiasts who want precise control over their sound. Whether you're enhancing music files, preparing audio for distribution or experimenting with creative effects, WaveShaper provides all the tools you need in a clean, intuitive interface. The application combines a professional 10-band parametric equalizer with studio-quality effects, dynamic compression, mastering tools and real-time spectrum analysis to help you achieve the perfect sound. Core audio effects and DSP stages are custom implementations built on peer-reviewed signal processing research, with third-party libraries used for audio I/O, encoding and metadata support.

### **Key Features**

- **10-Band Parametric Equalizer:** SVF-TPT topology filters with zero-delay feedback, adjustable Q-factor, multiple response types, 6/12/18/24/36/48 dB/oct HP/LP slopes and 44 built-in genre presets.
- **Audio Effects Suite:** FDN-based reverb with stereo width and diffusion control, Thiran-interpolated delay with filtered feedback, ADAA saturation, BBD-modeled chorus and flanger, PolyBLEP-driven modulation with switchable LFO waveform.
- **Dynamic Compression:** Logarithmic gain computation, continuous knee width, adjustable envelope smoothing, multiband compression with per-band threshold and ratio, integrated noise gate / expander.
- **Mastering Suite:** Loudness meter (Peak, True Peak, LUFS), five-style brick-wall limiter, stereo imaging, exciter and tape saturation with six purpose-built mastering presets.
- **Per-Track Audio Enhancement:** Five independent player sliders — Air Boost, Warmth, Presence, Harmonics and Stereo Width — layered on top of the preset selector.
- **Creative Sound Design:** Seven creative effects (Reverse, Stutter, Gate, Bitcrush, Lo-Fi, Ring Mod, Granular), each with its own parameter panel that appears when the effect is selected.
- **Spectrum Analyzer:** Seven display modes including Linear, Logarithmic, Smooth, Peak, RMS, Octave and Average Hold.
- **Audio Library:** Drag-and-drop import, multiple sort orders, favorites and seamless integration with the Medio download library.
- **High-Quality Export:** Export to `WAV`, `FLAC`, `MP3`, `AAC` or `OGG` with configurable normalization, bitrate, sample rate and bit depth.

> **Looking for in-depth documentation?** Every page, control and parameter is documented in [**FEATURES.md**](FEATURES.md) — read it for the full reference on how each part of the app works and what it does to your audio.

### **Supported Formats**

- **Input Formats:** `MP3`, `WAV`, `FLAC`, `WMA`, `AAC`, `M4A`, `OGG`
- **Output Formats:** `WAV`, `FLAC`, `MP3`, `AAC`, `OGG`

## **Table of Contents**

1. [System Requirements](#system-requirements)
2. [Third-Party Libraries](#third-party-libraries)
3. [Installation](#installation)
4. [Authentication and Arctisoft Hub](#authentication-and-arctisoft-hub)
5. [License Options and Benefits](#license-options-and-benefits)
6. [Getting Started Guide](#getting-started-guide)
7. [Customization](#customization)
8. [Updating Software](#updating-software)
9. [Copyright](#copyright)
10. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit) version 1809 or later
- **Processor:** Intel Core i3-8100 or AMD Ryzen 3 2200G with 4 cores at 3.0 GHz
- **RAM:** 8 GB
- **Graphics:** DirectX 11 compatible graphics card
- **Storage:** 400 MB of free disk space plus additional space for audio files
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**
- **Audio:** WaveOut, WASAPI, DirectSound or ASIO compatible audio device

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit) version 21H2 or later
- **Processor:** Intel Core i5-10400 or AMD Ryzen 5 3600 with 6 cores, 3.6 GHz or higher
- **RAM:** 16 GB or higher
- **Graphics:** Dedicated GPU for smooth visualization rendering
- **Storage:** 500 MB of free disk space on SSD plus additional space for audio files
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**
- **Audio:** Low-latency WASAPI Exclusive or ASIO audio interface for professional monitoring

**Note:** WaveShaper is designed exclusively for Windows. The .NET 10.0 Runtime is bundled directly in the installer, allowing WaveShaper to start immediately without requiring separate installation.

## **Third-Party Libraries**

WaveShaper uses several third-party libraries for audio I/O, encoding and metadata. All DSP — equalizer, reverb, delay, saturation, modulation, compression, mastering, creative effects, enhancement — is implemented in-house on top of NAudio's sample provider architecture. Pitch and tempo processing is implemented in-house on top of WaveShaper's own realtime providers.

| Library | Version | Used For | License |
|---|---|---|---|
| [NAudio](https://github.com/naudio/NAudio) | 2.2.1 | Audio I/O, file decoding, WaveOut/WASAPI/ASIO/DirectSound device output, sample provider pipeline | MIT |
| [NAudio.Lame](https://github.com/Corey-M/NAudio.Lame) | 2.1.0 | MP3 encoding through the LAME encoder | MIT (LAME: LGPL) |
| [CUETools.Codecs.FLAKE-Reloaded](https://github.com/teekay/FLACTools) | 1.0.1 | Pure-.NET FLAC encoding, no external FFmpeg needed | LGPL 2.1 |
| [TagLibSharp](https://github.com/mono/taglib-sharp) | 2.3.0 | Reading and writing audio metadata tags on export | LGPL |
| [Newtonsoft.Json](https://github.com/JamesNK/Newtonsoft.Json) | 13.0.4 | Settings, preset files and configuration serialization | MIT |
| [OggVorbisEncoder](https://github.com/SteveLillis/.NET-Ogg-Vorbis-Encoder) | 1.2.2 | Pure-managed Ogg Vorbis export | MIT |

For more details about these libraries, including their capabilities and licensing, check their official documentation. If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/issues) on GitHub.

## **Installation**

1. Download the latest release from the [Releases](https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/releases) page.
2. Run the installer and follow the setup wizard.
3. The installer will prompt you to install [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) (recommended for cloud sync and license management).
4. Launch WaveShaper from the Start Menu or Desktop shortcut.

## **Authentication and Arctisoft Hub**

WaveShaper integrates with [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) for account management, cloud sync and license activation. You can use WaveShaper without signing in, but some features require an Arctisoft account.

### Without Signing In

Launch WaveShaper without Arctisoft Hub to use it immediately. All core features including the equalizer, effects, compression and playback are available. Settings and presets are stored locally on your device.

### Signing In Through Arctisoft Hub

To unlock cloud sync and Premium features, sign in through [Arctisoft Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub):

1. **Install Arctisoft Hub** and sign in or create an account
2. **Open WaveShaper** - it detects your Hub session automatically
3. **Your cloud profile loads**, syncing settings and preferences

**On Additional Devices:**
- Install Arctisoft Hub and sign in with the same account
- Open WaveShaper - your profile syncs automatically from the cloud
- All settings and preferences are available on the new device

**Important Notes:**
- **Basic License:** All core audio processing features are available for free. Settings are stored locally.
- **Premium License:** Unlocks professional export features, mastering suite, pitch/tempo export, hi-res audio and cloud preset sync.
- **Profile Persistence:** All profiles are retained until the user manually deletes their account.

## **License Options and Benefits**

WaveShaper offers two license tiers:

- **Basic (Free):** Full audio workflow — EQ, reverb, delay, saturation, basic modulation (Tremolo / Vibrato / Pan), two creative effects (Reverse, Bitcrush), single-band compression with gate + limiter, full player + visualization, WAV / MP3 / FLAC / OGG export up to 48 kHz / 24-bit with Peak −1 dB normalization
- **Premium (€14.99 one-time):** Pro upgrades — Mastering Suite, multi-band compression (per-band threshold/ratio), time-stretch + pitch-shift, advanced modulation (Chorus / Phaser / Flanger), advanced creative FX (Stutter / Gate / Lo-Fi / Ring Mod / Granular), AAC export, LUFS normalization (−14 / −16 / −23), hi-res sample rates (up to 192 kHz), 32-bit float export and cloud preset sync

License keys are delivered via email after purchase. Purchases are processed through a secure Stripe checkout, and keys are typically delivered within minutes.

| Feature | Basic | Premium |
|---------|:-----:|:-------:|
| **EQUALIZER** | | |
| 10-Band EQ (all bands, ranges, response types) | ✓ | ✓ |
| HP/LP filter slope (6 / 12 / 18 / 24 / 36 / 48 dB/oct) | ✓ | ✓ |
| 44 built-in presets (all quality levels) | ✓ | ✓ |
| Unlimited custom presets | ✓ | ✓ |
| Preset Manual / Keyword / Analyze modes | ✓ | ✓ |
| **EFFECTS - REVERB, DELAY, SATURATION** | | |
| Reverb — 6 types, plus stereo width, diffusion, pre-delay, decay, room size, dampening, mix | ✓ | ✓ |
| Delay — 6 modes with feedback high-cut + low-cut filters | ✓ | ✓ |
| Saturation — 5 ADAA-anti-aliased models with drive / mix / output | ✓ | ✓ |
| Per-panel enable/bypass on every effect block | ✓ | ✓ |
| **COMPRESSOR** | | |
| Compressor with Ratio, Threshold, Attack, Release, Makeup Gain | ✓ | ✓ |
| Soft Knee, Dry/Wet Mix, Sidechain, Auto-Release, Lookahead | ✓ | ✓ |
| Envelope smoothing + continuous knee-width controls | ✓ | ✓ |
| Gate / Expander (Threshold, Range, Attack, Release, Hold) | ✓ | ✓ |
| Brick-wall Limiter | ✓ | ✓ |
| Multi-band Compression (4-Band, per-band threshold + ratio) | Preview only | ✓ |
| **MASTERING SUITE** | | |
| Professional Limiter (Lookahead, Ceiling, True Peak, 5 styles) | Preview only | ✓ |
| Stereo Imaging (Width 0-200%, Mid/Side Balance) | Preview only | ✓ |
| Exciter & Tape Saturation (Harmonic Enhancement) | Preview only | ✓ |
| LUFS Metering (Peak, True Peak, Integrated LUFS) | ✓ | ✓ |
| Mastering Presets (Streaming, Broadcast, CD, Vinyl, Loud) | Preview only | ✓ |
| Output Gain & Target Loudness (-24 to -6 LUFS) | Preview only | ✓ |
| **TIME STRETCH & PITCH SHIFT** | | |
| Pitch Shift (±12 Semitones) | Preview only | ✓ |
| Time Stretch / Tempo (0.25x - 4.0x) | Preview only | ✓ |
| 5 Processing Modes (Standard to Maximum Quality) | Preview only | ✓ |
| 5 Algorithms (PSOLA, WSOLA, Phase Vocoder, Granular, Harmonic-Percussive) | Preview only | ✓ |
| **MODULATION** | | |
| Tremolo, Vibrato, Pan Modulation (Rate, Depth, LFO Shape) | ✓ | ✓ |
| Chorus (Rate, Depth, LFO Shape, Voices 2-6, Chorus Mix) | Preview only | ✓ |
| Phaser, Flanger (Rate, Depth, LFO Shape) | Preview only | ✓ |
| **CREATIVE FX** | | |
| Normal (Bypass) | ✓ | ✓ |
| Reverse (Reverse Mix) | ✓ | ✓ |
| Bitcrush (Bit Depth, Sample Rate, Crush Mix, Overdrive) | ✓ | ✓ |
| Stutter (Length, Repeats) | Preview only | ✓ |
| Gate (Rate, Threshold, Shape, Attack, Release) | Preview only | ✓ |
| Lo-Fi (Amount, Mix) | Preview only | ✓ |
| Ring Mod (Frequency, Amount) | Preview only | ✓ |
| Granular (Amount) | Preview only | ✓ |
| **PLAYER & VISUALIZATION** | | |
| Full transport controls (Play, Stop, Previous, Next) | ✓ | ✓ |
| 5 Playback Modes (Normal, Shuffle, Repeat One, Repeat All, Smart Mix) | ✓ | ✓ |
| 5 Audio Modes (Standard, Night Mode, 3D Audio, Cinema, Concert) | ✓ | ✓ |
| 5 individual Enhancement sliders (Air Boost, Warmth, Presence, Harmonics, Stereo Width) | ✓ | ✓ |
| 8 Visualizations (Waveform, Pulse, Center Bars, LED Matrix, DNA Helix, Particle Field, Shockwave, Flames) | ✓ | ✓ |
| Crossfade, Dynamic Range, Stereo Balance, Mono Check | ✓ | ✓ |
| **SPECTRUM ANALYZER** | | |
| 7 Display Modes (Linear, Logarithmic, Smooth, Peak, RMS, Octave, Avg Hold) | ✓ | ✓ |
| **AUDIO EXPORT** | | |
| WAV (Lossless) | ✓ | ✓ |
| MP3 (all bitrates up to 320 kbps) | ✓ | ✓ |
| FLAC (Lossless) | ✓ | ✓ |
| OGG Vorbis | ✓ | ✓ |
| AAC | - | ✓ |
| Peak −1 dB normalization | ✓ | ✓ |
| LUFS normalization (−14 Streaming, −16 Apple, −23 Broadcast) | - | ✓ |
| Sample rates up to 48 kHz | ✓ | ✓ |
| Sample rates above 48 kHz (88.2 / 96 / 176.4 / 192 kHz) | - | ✓ |
| Bit depth 16-bit / 24-bit | ✓ | ✓ |
| Bit depth 32-bit float | - | ✓ |
| **AUDIO ENGINE** | | |
| Standard (WaveOut), WASAPI Shared, WASAPI Exclusive, DirectSound, ASIO | ✓ | ✓ |
| Buffer Size (64-2048 samples) | ✓ | ✓ |
| All Dithering types (RPDF, TPDF, Noise Shaping) | ✓ | ✓ |
| DSP Threads (1-10) | ✓ | ✓ |
| 4 Audio Quality levels (Low/Fast to Ultra) | ✓ | ✓ |
| **LIBRARY** | | |
| Audio library with drag-and-drop import (200 default, up to 600) | ✓ | ✓ |
| Sorting, Favorites, Medio Folder and Music Folder sources | ✓ | ✓ |
| Cloud-synced settings (requires Hub sign-in) | ✓ | ✓ |
| Cloud preset sync | - | ✓ |
| **CUSTOMIZATION** | | |
| 7 Color themes | ✓ | ✓ |
| Right-click "Reset Module" on every sidebar option box | ✓ | ✓ |
| **PRICE** | **Free** | **€14.99** (one-time) |

"Preview only" means the effect is fully functional during playback but excluded from the exported file for Basic users. When exporting, a dialog offers: Cancel / Upgrade / Export without Premium Effects.

Each Arctisoft-Studio product has its own license. A WaveShaper Premium key activates WaveShaper Premium features only. Redeem and manage keys through the [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub) Licenses page; WaveShaper detects the shared Hub session and license status automatically.

Multiple payment methods are accepted including Card, Klarna, EPS, Bancontact and iDEAL. Since licenses are digital products, refunds are generally **not available** once the key has been delivered. However, if you encounter any issues during the activation process, please don't hesitate to reach out for assistance.

## **Getting Started Guide**

### **Step 1: Import Your Audio**

1. Launch WaveShaper and navigate to the **Library** tab.
2. Import your audio file by dragging it onto the audio library or clicking **Import Audio**.
3. Double-click the imported file to load it for processing.

### **Step 2: Shape Your Sound with EQ**

1. Navigate to the **Equalizer** tab.
2. Select a preset that matches your music genre, or start with **Flat** for a neutral baseline.
3. Adjust individual bands by dragging the sliders up (boost) or down (cut).
4. Use the Q-Factor control for narrow surgical adjustments or wide tonal changes.
5. For high-pass or low-pass filters, pick a slope (6 / 12 / 18 / 24 / 36 / 48 dB/oct) from the Advanced EQ panel.
6. Preview your changes using the **Play Audio** button.

### **Step 3: Add Effects**

1. Open the **Effects** tab.
2. Add space with reverb — pick a type and dial in pre-delay, decay, room size, dampening, stereo width and diffusion.
3. Create echoes with delay — choose a mode, set time and feedback, and shape the feedback path with the High-Cut / Low-Cut filters.
4. Add warmth with saturation — pick a model and dial in the drive.
5. Experiment with modulation (the panel changes its controls based on the type you select in the sidebar) and creative effects.
6. Disable any panel you're not using via the checkbox in its top-right corner.

### **Step 4: Control Dynamics with Compression**

1. Go to the **Compress** tab.
2. Select a preset based on your material (Vocal, Drums, Bass, Master).
3. Fine-tune threshold and ratio for the amount of compression.
4. Adjust attack, release, envelope smoothing and knee width to shape the response.
5. For complex material, enable the **Multiband** panel and set per-band thresholds and ratios.
6. Use the Gate/Expander to clean up noise between phrases.

### **Step 5: Master Your Audio**

1. Navigate to the **Mastering** tab.
2. Select a mastering preset matching your delivery target (Streaming, Broadcast, CD).
3. Enable the limiter, pick a Style (Transparent / Punchy / Aggressive / Brickwall / Soft Clip) inline in the panel, and set the ceiling.
4. Adjust stereo width and add exciter or tape saturation for character.
5. Monitor loudness levels on the mastering meter to meet platform standards.

### **Step 6: Export Your Processed Audio**

1. Return to the **Library** tab.
2. Select your audio file and click **Export Audio**.
3. Choose output format (`WAV`, `FLAC`, `MP3`, `AAC` or `OGG`).
4. Configure normalization and quality settings in Settings if needed.
5. Click **Export** and select your destination folder.

For deep parameter-by-parameter explanations of every page and control, see [**FEATURES.md**](FEATURES.md).

## **Customization**

### **Color Themes**

Personalize WaveShaper with seven color themes that completely transform the application's appearance. Each theme shifts the entire color palette including backgrounds, borders, accents and visualizations:

- **Ocean Blue** - Deep blue tones (default)
- **Emerald Mist** - Natural emerald greens
- **Sunset Orange** - Warm amber hues
- **Nebula Night** - Rich amethyst purples
- **Cherry Blossom** - Soft rose and pink tones
- **Ruby Ember** - Deep cherry reds
- **Phantom Frost** - Bright cyan and teal

Changes apply immediately without restart.

### **Audio Quality and Performance**

Optimize WaveShaper for your hardware through the Settings page:

- **Audio Quality:** Choose from Low (Fast), Medium, High (Best) or Ultra processing quality
- **DSP Threads:** Allocate 1-10 processing threads based on your CPU capabilities
- **Buffer Size:** Adjust from 64 to 2048 samples to balance latency and stability
- **Audio Driver:** Select Standard WaveOut, WASAPI Shared (compatible), WASAPI Exclusive (low-latency), DirectSound or ASIO

### **Reset Individual Options**

Right-clicking any option box in the right-hand sidebar (Time Display, Performance, FFT Size, Mastering Chain, etc.) opens the same two-item context menu used on every main panel: **Reset Module** and a greyed-out **Disable Module**. Selecting **Reset Module** reverts just that single setting to its factory value without touching the rest of your configuration — no need to factory-reset the whole page or app. **Disable Module** is intentionally disabled on sidebar option boxes (they have no bypass concept) so the menu layout stays consistent across the whole shell.

## **Updating Software**

WaveShaper is updated through [Arctisoft Studio Hub](https://github.com/BerndHagen/Arctisoft-Studio-Hub). When a new version is available, the Hub detects it automatically and handles the download and installation process. The application restarts with the new version after installation.

For manual updates or first-time installation, download the latest installer from the [Releases](https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/releases) page and run it. The installer handles all dependencies and creates Start Menu and optional Desktop shortcuts.

## **Copyright**

This software is the intellectual property of the Author and is protected by international copyright laws.

1. **License:** You are granted a non-exclusive, non-transferable license to use the software for personal and commercial purposes.

2. **Modifications Prohibited:** Modification, decompiling, reverse-engineering or derivative work is prohibited without prior written consent.

3. **Attribution:** When redistributing, appropriate credit to the Author is required, including a link to the original source.

4. **Third-Party Libraries:** WaveShaper uses NAudio (MIT), NAudio.Lame (MIT; bundled LAME encoder LGPL), CUETools.Codecs.FLAKE-Reloaded (LGPL 2.1), TagLibSharp (LGPL), Newtonsoft.Json (MIT) and OggVorbisEncoder (MIT). Please review and comply with their respective licenses.

5. **Warranty Disclaimer:** WaveShaper is provided *"as is,"* without warranties of any kind. The Author assumes no liability for damages resulting from use.

6. **Limitation of Liability:** The Author is not responsible for any indirect, special, incidental or consequential damages arising from use of the software.

7. **Termination:** The license may be terminated if these terms are violated. Upon termination, all use must cease and copies deleted.

By using WaveShaper, you agree to these terms and conditions.

## **Screenshots**

Preview WaveShaper's interface and features before downloading. Note that future updates may introduce additional functionality.

<table>
  <tr>
    <th>WaveShaper - Dashboard</th>
    <th>WaveShaper - Equalizer</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-dashboard.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-dashboard.png" alt="WaveShaper Dashboard" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-equalizer.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-equalizer.png" alt="WaveShaper Equalizer" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Library</th>
    <th>WaveShaper - Player</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-library.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-library.png" alt="WaveShaper Library" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-player.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-player.png" alt="WaveShaper Player" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Effects</th>
    <th>WaveShaper - Mastering</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-effects.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-effects.png" alt="WaveShaper Effects" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-mastering.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-mastering.png" alt="WaveShaper Mastering" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Compressor</th>
    <th>WaveShaper - Presets</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-compressor.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-compressor.png" alt="WaveShaper Compressor" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-presets.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processing-Studio/raw/main/images/screenshot-presets.png" alt="WaveShaper Presets" width="450"></a></td>
  </tr>
</table>
