<p align="center">
  <img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_waveshaper.png" alt="WaveShaper Logo" width="128" />
</p>
<h1 align="center">WaveShaper - Audio Processor</h1>
<p align="center">
  <b>Shape your sound with professional-grade audio processing, EQ mastering and real-time visualization.</b><br>
  <b>Experience a powerful, intuitive audio workstation optimized for precision and performance.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/WaveShaper-Audio-Processor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-blue?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">
</p>

**WaveShaper** is a professional audio processing application designed for musicians, producers and audio enthusiasts who want precise control over their sound. Whether you're enhancing music files, preparing audio for distribution or experimenting with creative effects, WaveShaper provides all the tools you need in a clean, intuitive interface. The application combines a professional 10-band parametric equalizer with studio-quality effects, dynamic compression and real-time visualization to help you achieve the perfect sound.

### **Key Features**

- **10-Band Equalizer:** Fine-tune your audio with professional-grade parametric EQ, featuring adjustable Q-factor, multiple response types and 21 built-in presets covering all major music genres.
- **Audio Effects Suite:** Transform your sound with six reverb environments, multiple delay modes, tempo-independent time stretching, modulation effects and creative sound design tools.
- **Dynamic Compression:** Control audio dynamics with three compressor models, intelligent detection modes and purpose-built presets for vocals, drums, bass and mastering.
- **Spectrum Analyzer:** Visualize frequency content in real-time with configurable FFT sizes, multiple display modes and peak hold functionality for precise audio monitoring.
- **Project Library:** Organize and manage your audio files with drag-and-drop import, multiple sorting options and seamless integration with Medio download library.
- **High-Quality Export:** Export processed audio to `WAV` or `MP3` with automatic metadata embedding and configurable sample rate and bit depth settings.

### **Supported Formats**

WaveShaper handles a wide range of audio formats for both import and export:

- **Input Formats:** `MP3`, `WAV`, `FLAC`, `WMA`, `AAC`, `M4A`
- **Output Formats:** `WAV`, `MP3`

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
3. [Understanding the Equalizer](#understanding-the-equalizer)
   - [Frequency Bands Explained](#frequency-bands-explained)
   - [Quality Levels](#quality-levels)
   - [EQ Response Types](#eq-response-types)
   - [Built-in Presets](#built-in-presets)
4. [Audio Effects Explained](#audio-effects-explained)
   - [Reverb and Space](#reverb-and-space)
   - [Delay Effects](#delay-effects)
   - [Time Stretching](#time-stretching)
   - [Stereo Imaging](#stereo-imaging)
   - [Modulation](#modulation)
   - [Creative Effects](#creative-effects)
5. [Dynamic Compression Guide](#dynamic-compression-guide)
   - [What is Compression](#what-is-compression)
   - [Compressor Types](#compressor-types)
   - [Detection Modes](#detection-modes)
   - [Compression Presets](#compression-presets)
6. [Visualization and Monitoring](#visualization-and-monitoring)
7. [Managing Your Projects](#managing-your-projects)
8. [Audio Playback](#audio-playback)
9. [Configuring Audio Settings](#configuring-audio-settings)
10. [Getting Started Guide](#getting-started-guide)
11. [Customization](#customization)
12. [Updating Software](#updating-software)
13. [Copyright](#copyright)
14. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit) version 1809 or later
- **Processor:** Intel Core i3-8100 or AMD Ryzen 3 2200G with 4 cores at 3.0 GHz
- **RAM:** 8 GB
- **Graphics:** DirectX 11 compatible graphics card
- **Storage:** 200 MB of free disk space plus additional space for audio files
- **Software:** .NET 10.0 Runtime
  - [Download .NET 10.0 Runtime](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)
- **Audio:** ASIO, WASAPI or DirectSound compatible audio device

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit) version 21H2 or later
- **Processor:** Intel Core i5-10400 or AMD Ryzen 5 3600 with 6 cores, 3.6 GHz or higher
- **RAM:** 16 GB or higher
- **Graphics:** Dedicated GPU for smooth visualization rendering
- **Storage:** 500 MB of free disk space on SSD plus additional space for audio files
- **Software:** .NET 10.0 Runtime
  - [Download .NET 10.0 Runtime](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)
- **Audio:** Low-latency ASIO audio interface for professional monitoring

## **Third-Party Libraries**

WaveShaper uses several third-party libraries to handle audio processing, encoding and metadata operations.

### NAudio

**NAudio** is a comprehensive .NET audio library that provides the core audio functionality for WaveShaper. It handles file decoding, real-time playback, audio device communication and provides the sample processing infrastructure that makes effects and equalization possible.

- **Version:** 2.2.1
- **Website:** [NAudio GitHub Repository](https://github.com/naudio/NAudio)
- **License:** NAudio is licensed under the MIT License, allowing free use, distribution, and modification.

### NAudio.Lame

**NAudio.Lame** enables high-quality MP3 encoding through the LAME encoder. When exporting to MP3, this library ensures your audio is compressed with industry-standard quality while maintaining the smallest file size possible.

- **Version:** 2.1.0
- **Website:** [NAudio.Lame GitHub Repository](https://github.com/Corey-M/NAudio.Lame)
- **License:** NAudio.Lame is licensed under the LGPL.

### SoundTouch.Net

**SoundTouch.Net** is a .NET wrapper for the SoundTouch audio processing library. It powers the time stretching and pitch shifting features, using advanced algorithms to change tempo without affecting pitch or shift pitch without changing tempo.

- **Version:** 2.1.2
- **Website:** [SoundTouch Official Website](https://www.surina.net/soundtouch/)
- **License:** SoundTouch.Net is licensed under the LGPL v2.1.

### TagLibSharp

**TagLibSharp** handles metadata operations, allowing WaveShaper to read and write audio file tags. When you export a processed file, this library embeds title, artist, album and other metadata directly into the audio file.

- **Version:** 2.3.0
- **Website:** [TagLibSharp GitHub Repository](https://github.com/mono/taglib-sharp)
- **License:** TagLibSharp is licensed under the LGPL.

### Additional Information

For more details about these libraries, including their capabilities and licensing, check their official documentation. If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/WaveShaper-Creative-Audio-Editor/issues) on GitHub.

## **Understanding the Equalizer**

An equalizer is one of the most powerful tools for shaping your audio. It allows you to boost or cut specific frequency ranges, making instruments or voices more prominent, removing unwanted rumble or adding brightness and clarity. WaveShaper's 10-band parametric equalizer provides precise control over the entire audible spectrum.

### **Frequency Bands Explained**

The equalizer divides the audio spectrum into ten bands, each targeting a specific frequency range. Understanding what each band affects helps you make better mixing decisions:

| Band | Frequency | What It Controls |
|------|-----------|------------------|
| Band 1 | `32 Hz` | Sub-bass, the lowest frequencies you feel more than hear. Adds rumble and weight. |
| Band 2 | `64 Hz` | Bass fundamentals. Controls the punch and power of kick drums and bass instruments. |
| Band 3 | `125 Hz` | Upper bass. Adds warmth but can also cause muddiness if boosted too much. |
| Band 4 | `250 Hz` | Low-midrange. Affects the body of vocals and the fullness of guitars. |
| Band 5 | `500 Hz` | Midrange. The core of most instruments and voices. Crucial for clarity. |
| Band 6 | `1 kHz` | Upper-midrange. Affects presence and can make sounds feel closer or farther away. |
| Band 7 | `2 kHz` | Presence range. Boosting here adds bite to guitars and clarity to vocals. |
| Band 8 | `4 kHz` | Brilliance. Enhances consonants in speech and attack in percussion. |
| Band 9 | `8 kHz` | High frequencies. Adds air and sparkle to the overall mix. |
| Band 10 | `16 kHz` | Ultra-high frequencies. Adds shimmer and openness, though less audible on lower-quality systems. |

Each band also features an adjustable **Q-Factor** (ranging from `0.1` to `5.0`) that controls bandwidth. A low Q value affects a wide range of frequencies around the center point, while a high Q value makes surgical, narrow adjustments.

### **Quality Levels**

WaveShaper offers four quality levels that determine how much gain adjustment is available on each band:

- **Standard** (±6 dB): Suitable for subtle corrections and gentle tone shaping without risk of distortion.
- **Enhanced** (±12 dB): The default setting, providing enough headroom for most mixing tasks.
- **Professional** (±18 dB): For significant frequency corrections when audio needs major reshaping.
- **Extreme** (±24 dB): Maximum adjustment range for sound design and creative frequency manipulation.

### **EQ Response Types**

Three response curves are available, each with different characteristics:

- **Smooth Curve:** Gradual transitions between bands for natural-sounding adjustments.
- **Sharp Digital:** Precise, accurate response for surgical corrections.
- **Analog Warmth:** Emulates the gentle rolloff and harmonic character of vintage hardware equalizers.

### **Built-in Presets**

WaveShaper includes 21 professionally-tuned presets to help you get started quickly:

**Genre Presets:** Each genre preset is optimized for the typical frequency balance of that music style.
- Rock, Pop, Jazz, Classical, Hip Hop, Electronic, R&B, Metal, Reggae, Country, Latin, Acoustic

**Utility Presets:** Designed for specific corrective or enhancement purposes.
- **Flat:** Neutral starting point with no adjustments
- **Bass Boost / Treble Boost:** Quick low or high frequency enhancement
- **Vocal:** Emphasizes the presence range for clearer voice
- **Bass Reducer:** Cuts low frequencies for cleaner sound on small speakers
- **Loudness:** Classic loudness curve for low-volume listening
- **Headphones:** Optimized for headphone playback
- **Small Speakers:** Compensates for speakers that lack bass response
- **Live:** Adds presence and energy typical of live performances

## **Audio Effects Explained**

Beyond equalization, WaveShaper provides a comprehensive suite of audio effects that can transform your sound from subtle enhancement to dramatic creative manipulation.

### **Reverb and Space**

Reverb simulates the natural reflections of sound in physical spaces. When you clap your hands in a large hall, you hear the sound bounce off walls and decay over time. WaveShaper offers six reverb environments:

- **Room:** Small room ambience, subtle and natural
- **Hall:** Concert hall with longer decay for orchestral depth
- **Cathedral:** Very large space with extended reverb tail
- **Chamber:** Studio recording room simulation
- **Plate:** Classic studio reverb with smooth, dense decay
- **Spring:** Vintage spring reverb character

Each reverb type can be adjusted with **Room Size** (how large the simulated space feels) and **Dampening** (how quickly high frequencies decay).

### **Delay Effects**

Delay creates echoes by repeating the audio signal after a set time interval. WaveShaper provides six delay modes:

- **Simple:** Single repeat for basic echo effects
- **Ping-Pong:** Alternates between left and right speakers for spacious stereo effects
- **Multi-Tap:** Multiple delay times create rhythmic patterns
- **Filtered:** Delay with frequency filtering for darker, more vintage echoes
- **Stereo:** Independent delay times for each channel
- **Reverse:** Reversed delay trails for creative sound design

Delay parameters include **Delay Time** (up to 999ms) and **Feedback** (controls how many times the delay repeats).

### **Time Stretching**

Time stretching allows you to change the tempo of audio without affecting its pitch, or shift pitch without changing tempo. This is essential for tempo matching, creative effects and correcting pitch issues.

**Processing Modes:**
- Standard, High Quality, Best Quality, Low Latency, Maximum Quality

**Algorithms:**
- **PSOLA:** Best for monophonic sources like vocals
- **WSOLA:** Good general-purpose algorithm
- **Phase Vocoder:** Preserves harmonic content well
- **Granular:** Suitable for extreme stretching
- **Harmonic-Percussive:** Separates and processes tonal and rhythmic content differently

**Speed Range:** `0.25x` to `4.0x` playback speed
**Pitch Shift:** `-12` to `+12` semitones (one full octave up or down)

### **Stereo Imaging**

Control the width and position of your stereo field:

- **Mono:** Collapses stereo to center, useful for checking mono compatibility
- **Narrow Stereo:** Reduced width for focused sound
- **Normal Stereo:** Original stereo image
- **Wide Stereo:** Expanded stereo field for bigger, more immersive sound

### **Modulation**

Modulation effects add movement and animation to your audio:

- **No Modulation:** Bypass mode
- **Tremolo:** Volume modulation creates a wavering effect
- **Vibrato:** Pitch modulation adds subtle pitch variation
- **Pan Modulation:** Stereo position moves left and right automatically

### **Creative Effects**

For more experimental sound design:

- **Normal:** No effect applied
- **Reverse:** Plays audio backwards
- **Stutter:** Creates rhythmic chopping effects
- **Gate:** Cuts audio below a threshold for rhythmic silence
- **Bitcrush:** Reduces bit depth for lo-fi, digital distortion character

## **Dynamic Compression Guide**

### **What is Compression**

Dynamic compression is essential for controlling the volume differences in audio. Without compression, quiet parts might be too soft while loud parts distort or overpower the mix. A compressor automatically reduces the volume of signals that exceed a certain threshold, creating a more consistent and professional sound.

Think of compression like an automatic volume control that turns down the loud parts. This allows you to then raise the overall level, making quiet details more audible while preventing peaks from distorting.

### **Compressor Types**

WaveShaper offers three compressor models, each with distinct sonic characteristics:

- **VCA (Voltage Controlled Amplifier):** Fast, precise and transparent compression. VCA compressors respond quickly to transients and are excellent for maintaining clarity while controlling dynamics. Ideal for drums, full mixes and any material requiring clean, accurate compression.

- **FET (Field Effect Transistor):** Aggressive, punchy compression with harmonic color. FET compressors add subtle distortion and excitement to the signal, making them popular for vocals, bass and drums when you want added character and bite.

- **Opto (Optical):** Smooth, musical compression with natural-sounding gain reduction. Optical compressors have slower response times that gently follow the program material, perfect for vocals, bass and any source where you want compression that remains invisible.

### **Detection Modes**

The detection mode determines how the compressor measures the incoming signal:

- **Peak:** Responds to instantaneous signal peaks, providing fast, transient-catching compression.
- **RMS (Root Mean Square):** Responds to average signal level, creating smoother, more musical compression.
- **Hybrid:** Combines peak and RMS detection for balanced control.

### **Compression Presets**

Six purpose-built presets provide optimized starting points:

| Preset | Threshold | Ratio | Attack | Release | Makeup | Mix | Best For |
|--------|-----------|-------|--------|---------|--------|-----|----------|
| Vocal | -18 dB | 3.0:1 | 3 ms | 100 ms | 3 dB | 100% | Spoken word, singing |
| Drums | -10 dB | 4.0:1 | 1 ms | 50 ms | 2 dB | 100% | Drum loops, percussion |
| Bass | -15 dB | 3.0:1 | 10 ms | 200 ms | 4 dB | 100% | Bass instruments |
| Master | -12 dB | 2.0:1 | 5 ms | 150 ms | 2 dB | 85% | Full mixes |
| Gentle | -24 dB | 1.5:1 | 10 ms | 300 ms | 1 dB | 70% | Subtle leveling |
| Custom | — | — | — | — | — | — | Your own settings |

**Advanced Features:**
- **Sidechain Filtering:** High-pass filter prevents bass frequencies from triggering excessive compression
- **Multiband:** Compress different frequency ranges independently
- **Auto Makeup Gain:** Automatically compensates for gain reduction
- **Lookahead:** Anticipates peaks for cleaner transient handling

## **Visualization and Monitoring**

### **Spectrum Analyzer**

The real-time spectrum analyzer displays the frequency content of your audio, helping you identify problematic frequencies, verify EQ adjustments and ensure a balanced mix.

**FFT Sizes:** `2048`, `4096`, `8192`, `16384` samples. Larger FFT sizes provide higher frequency resolution but slower response.

**Display Modes:**
- **Linear:** Equal spacing across frequencies
- **Logarithmic:** More resolution in lower frequencies (matches human hearing)
- **Smooth:** Averaged display for easier reading
- **Peak:** Shows maximum values with decay
- **RMS:** Shows average energy levels

### **Activity Dashboard**

The Dashboard tracks your usage patterns and provides an overview of your audio processing activities. View your session history across 7, 14, 21, 28 or 35 day periods to monitor your workflow and productivity.

## **Managing Your Projects**

The Project Library is your central hub for organizing audio files. By default, you can store up to 200 projects, though this limit can be increased in settings.

**Importing Audio:**
- Drag and drop files directly onto the library
- Use the Import button to browse for files
- Files are automatically analyzed for format, duration and sample rate

**Sorting Options:**
- Name A-Z / Name Z-A
- Largest Size / Smallest Size
- Newest Date / Oldest Date

**Medio Integration:** If you have the Medio Universal Downloader installed, WaveShaper can access your Medio download library directly. This allows you to quickly load audio extracted from videos without navigating through folders.

## **Audio Playback**

The Player provides full transport controls for auditioning your audio with applied effects:

- **Play/Pause/Stop:** Standard transport controls
- **Volume:** Master output volume with mute toggle
- **Stereo Balance:** Adjust left/right balance
- **Position Scrubbing:** Click and drag the waveform to seek

Real-time visualization shows the audio waveform and current playback position.

## **Configuring Audio Settings**

### **Sample Rates**

Higher sample rates capture more audio detail but result in larger file sizes:

- `44.1 kHz` — CD quality, standard for music
- `48 kHz` — Standard for video production
- `88.2 kHz` — High-resolution audio
- `96 kHz` — Professional studio standard
- `176.4 kHz` — Ultra high-resolution
- `192 kHz` — Maximum quality

### **Bit Depth**

Bit depth determines dynamic range and noise floor:

- **16-bit:** CD standard, 96 dB dynamic range
- **24-bit:** Professional standard, 144 dB dynamic range
- **32-bit Float:** Maximum headroom, prevents clipping during processing

### **Latency Modes**

Balance between responsiveness and stability:

- **Low:** Minimal delay, requires more CPU power
- **Standard:** Balanced setting for most systems
- **High:** Maximum stability, suitable for slower systems

### **Audio Modes**

- **Stereo:** Two-channel output
- **Mono:** Single-channel, useful for checking mono compatibility
- **Surround:** Multi-channel output when supported

## **Getting Started Guide**

### **Step 1: Import Your Audio**

1. Launch WaveShaper and navigate to the **Projects** tab.
2. Import your audio file by dragging it onto the project library or clicking **Import Project**.
3. Double-click the imported file to load it for processing.

### **Step 2: Shape Your Sound with EQ**

1. Navigate to the **Equalizer** tab.
2. Select a preset that matches your music genre, or start with **Flat** for a neutral baseline.
3. Adjust individual bands by dragging the sliders up (boost) or down (cut).
4. Use the Q-Factor control for narrow surgical adjustments or wide tonal changes.
5. Preview your changes using the **Play Audio** button.

### **Step 3: Add Effects**

1. Open the **Effects** tab.
2. Add space with reverb by selecting a room type and adjusting size and dampening.
3. Create echoes with delay by choosing a mode and setting time and feedback.
4. Experiment with time stretching, modulation and creative effects.

### **Step 4: Control Dynamics with Compression**

1. Go to the **Compressor** tab.
2. Select a preset based on your material (Vocal, Drums, Bass, Master).
3. Choose a compressor type that matches your desired character.
4. Fine-tune threshold and ratio for the amount of compression.
5. Adjust attack and release to shape transients.

### **Step 5: Export Your Processed Audio**

1. Return to the **Projects** tab.
2. Select your project and click **Export Project**.
3. Choose output format (`WAV` or `MP3`).
4. Set sample rate and bit depth as needed.
5. Click **Export** and select your destination folder.

## **Customization**

### **Color Themes**

Personalize WaveShaper with six color themes:

- Ocean Blue
- Forest Green
- Sunset Orange
- Purple Night
- Golden Hour
- Crimson Red

Changes apply immediately without restart.

### **Performance Modes**

Optimize WaveShaper for your hardware:

- **Power Saver:** Reduced visualizations and update rates for lower CPU usage
- **Balanced:** Standard performance for most systems
- **High Performance:** Maximum visual quality and responsiveness

## **Updating Software**

WaveShaper includes automatic update functionality that checks for new versions on startup. When an update is available, it downloads automatically and installs with minimal interruption. The application restarts with the new version after installation.

For manual updates, download the latest MSI installer from the repository and run it to replace existing files.

## **Copyright**

This software is the intellectual property of the Author and is protected by international copyright laws.

1. **License:** You are granted a non-exclusive, non-transferable license to use the software for personal and commercial purposes.

2. **Modifications Prohibited:** Modification, decompiling, reverse-engineering or derivative work is prohibited without prior written consent.

3. **Attribution:** When redistributing, appropriate credit to the Author is required, including a link to the original source.

4. **Third-Party Libraries:** WaveShaper uses NAudio (MIT), NAudio.Lame (LGPL), SoundTouch.Net (LGPL) and TagLibSharp (LGPL). Please review and comply with their respective licenses.

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
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-dashboard.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-dashboard.png" alt="WaveShaper Dashboard" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-equalizer.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-equalizer.png" alt="WaveShaper Equalizer" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Projects</th>
    <th>WaveShaper - Player</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-projects.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-projects.png" alt="WaveShaper Projects" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-player.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-player.png" alt="WaveShaper Player" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Effects</th>
    <th>WaveShaper - Compressor</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-effects.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-effects.png" alt="WaveShaper Effects" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-compressor.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-compressor.png" alt="WaveShaper Compressor" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Presets</th>
    <th>WaveShaper - Settings</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-presets.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-presets.png" alt="WaveShaper Presets" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-settings.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v1.0.0-waveshaper-settings.png" alt="WaveShaper Settings" width="450"></a></td>
  </tr>
</table>
