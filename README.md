<p align="center">
  <img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_waveshaper.png" alt="WaveShaper Logo" width="128" />
</p>
<h1 align="center">WaveShaper - Audio Processing Studio</h1>
<p align="center">
  <b>Shape your sound with professional-grade audio processing, EQ mastering and real-time visualization.</b><br>
  <b>Experience a powerful, intuitive audio workstation optimized for precision and performance.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/WaveShaper-Audio-Processor?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freeware-blue?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">
</p>

**WaveShaper** is a professional audio processing application designed for musicians, producers and audio enthusiasts who want precise control over their sound. Whether you're enhancing music files, preparing audio for distribution or experimenting with creative effects, WaveShaper provides all the tools you need in a clean, intuitive interface. The application combines a professional 10-band parametric equalizer with studio-quality effects, dynamic compression, mastering tools and real-time visualization to help you achieve the perfect sound.

### **Key Features**

- **10-Band Equalizer:** Fine-tune your audio with professional-grade parametric EQ, featuring adjustable Q-factor, multiple response types and 30 built-in presets covering all major music genres.
- **Audio Effects Suite:** Transform your sound with six reverb environments, multiple delay modes, saturation modeling, tempo-independent time stretching, modulation effects and creative sound design tools.
- **Dynamic Compression:** Control audio dynamics with adjustable ratio, threshold, attack and release. Includes a noise gate/expander for cleaning up recordings and soft/hard knee modes for precise dynamic control.
- **Mastering Suite:** Professional mastering tools including a loudness meter (Peak, True Peak, LUFS), configurable limiter, stereo imaging controls, exciter and tape saturation with purpose-built mastering presets.
- **Spectrum Analyzer:** Visualize frequency content in real-time with seven display modes including Linear, Logarithmic, Smooth, Peak, RMS, Octave and Average Hold for precise audio monitoring.
- **Project Library:** Organize and manage your audio files with drag-and-drop import, multiple sorting options, favorites and seamless integration with Medio download library.
- **High-Quality Export:** Export processed audio to `WAV`, `FLAC`, `MP3`, `AAC` or `OGG` with configurable normalization, bitrate, sample rate and bit depth settings.

### **Supported Formats**

WaveShaper handles a wide range of audio formats for both import and export:

- **Input Formats:** `MP3`, `WAV`, `FLAC`, `WMA`, `AAC`, `M4A`
- **Output Formats:** `WAV`, `FLAC`, `MP3`, `AAC`, `OGG`

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
   - [Custom Presets](#custom-presets)
   - [Preset Modes](#preset-modes)
4. [Audio Effects Explained](#audio-effects-explained)
   - [Time Stretching](#time-stretching)
   - [Reverb and Space](#reverb-and-space)
   - [Delay Effects](#delay-effects)
   - [Saturation](#saturation)
   - [Modulation](#modulation)
   - [Creative Effects](#creative-effects)
5. [Dynamic Compression Guide](#dynamic-compression-guide)
   - [What is Compression](#what-is-compression)
   - [Compression Presets](#compression-presets)
   - [Compressor Controls](#compressor-controls)
   - [Gate and Expander](#gate-and-expander)
6. [Mastering Suite](#mastering-suite)
   - [Mastering Meter](#mastering-meter)
   - [Mastering Presets](#mastering-presets)
   - [Limiter](#limiter)
   - [Stereo and Effects](#stereo-and-effects)
7. [Visualization and Monitoring](#visualization-and-monitoring)
8. [Managing Your Projects](#managing-your-projects)
9. [Audio Playback](#audio-playback)
   - [Playback Modes](#playback-modes)
   - [Audio Modes](#audio-modes)
   - [Player Controls](#player-controls)
10. [Preset Management](#preset-management)
    - [A/B Comparison](#ab-comparison)
    - [Preset Categories](#preset-categories)
11. [Configuring Audio Settings](#configuring-audio-settings)
    - [General Settings](#general-settings)
    - [Processing Settings](#processing-settings)
    - [Audio Engine](#audio-engine)
    - [Audio Devices](#audio-devices)
    - [Audio Export](#audio-export)
12. [Getting Started Guide](#getting-started-guide)
13. [Customization](#customization)
14. [Updating Software](#updating-software)
15. [Copyright](#copyright)
16. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit) version 1809 or later
- **Processor:** Intel Core i3-8100 or AMD Ryzen 3 2200G with 4 cores at 3.0 GHz
- **RAM:** 8 GB
- **Graphics:** DirectX 11 compatible graphics card
- **Storage:** 200 MB of free disk space plus additional space for audio files
- **Software:** .NET 10.0 Runtime
  - [Download .NET 10.0 Runtime](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)
- **Audio:** WASAPI or DirectSound compatible audio device

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit) version 21H2 or later
- **Processor:** Intel Core i5-10400 or AMD Ryzen 5 3600 with 6 cores, 3.6 GHz or higher
- **RAM:** 16 GB or higher
- **Graphics:** Dedicated GPU for smooth visualization rendering
- **Storage:** 500 MB of free disk space on SSD plus additional space for audio files
- **Software:** .NET 10.0 Runtime
  - [Download .NET 10.0 Runtime](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)
- **Audio:** Low-latency WASAPI Exclusive audio interface for professional monitoring

## **Third-Party Libraries**

WaveShaper uses several third-party libraries to handle audio processing, encoding and metadata operations.

### NAudio

**NAudio** is a comprehensive .NET audio library that provides the core audio functionality for WaveShaper. It handles file decoding, real-time playback, WASAPI and DirectSound audio device communication and provides the sample processing infrastructure that makes effects and equalization possible. WaveShaper uses NAudio's full ecosystem including ASIO support, WASAPI integration and WinMM audio subsystem.

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

- **Version:** 2.3.2
- **Website:** [SoundTouch Official Website](https://www.surina.net/soundtouch/)
- **License:** SoundTouch.Net is licensed under the LGPL v2.1.

### TagLibSharp

**TagLibSharp** handles metadata operations, allowing WaveShaper to read and write audio file tags. When you export a processed file, this library embeds title, artist, album and other metadata directly into the audio file.

- **Version:** 2.3.0
- **Website:** [TagLibSharp GitHub Repository](https://github.com/mono/taglib-sharp)
- **License:** TagLibSharp is licensed under the LGPL.

### Newtonsoft.Json

**Newtonsoft.Json** provides JSON serialization and deserialization for WaveShaper's settings, preset files and configuration management. It handles the storage and retrieval of user preferences, custom EQ presets and application state.

- **Version:** 13.0.4
- **Website:** [Newtonsoft.Json GitHub Repository](https://github.com/JamesNK/Newtonsoft.Json)
- **License:** Newtonsoft.Json is licensed under the MIT License.

### Additional Information

For more details about these libraries, including their capabilities and licensing, check their official documentation. If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/WaveShaper-Audio-Processor/issues) on GitHub.

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

WaveShaper includes 30 professionally-tuned presets to help you get started quickly:

**Genre Presets:** Each genre preset is optimized for the typical frequency balance of that music style.
- Rock, Pop, Jazz, Classical, Hip Hop, Electronic, R&B, Metal, Reggae, Country, Latin, Acoustic, Dance

**Utility Presets:** Designed for specific corrective or enhancement purposes.
- **Flat:** Neutral starting point with no adjustments
- **Bass Boost / Treble Boost:** Quick low or high frequency enhancement
- **Deep Bass:** Extreme sub-bass enhancement for bass-heavy music
- **Vocal:** Emphasizes the presence range for clearer voice
- **Bass Reducer:** Cuts low frequencies for cleaner sound on small speakers
- **Loudness:** Classic loudness curve for low-volume listening
- **Headphones:** Optimized for headphone playback
- **Small Speakers:** Compensates for speakers that lack bass response
- **Live:** Adds presence and energy typical of live performances
- **Powerful:** Aggressive V-shaped curve with boosted bass and treble

**Specialized Presets:** Optimized for specific content types and use cases.
- **Podcast:** Speech clarity optimization with enhanced mid-range
- **Spoken Word:** Similar to Podcast but with more aggressive voice focus
- **Gaming:** Spatial audio enhancement for games with balanced effects
- **Piano:** Warm mid-range focus for keyboard and piano music
- **Cinema:** Full spectrum enhancement for movie soundtracks and immersive audio
- **Soft:** Gentle, relaxed sound with reduced highs for easy listening

### **Custom Presets**

WaveShaper allows you to create and manage your own custom EQ presets:

**Automatic Custom Mode:**
When you select a preset and then manually adjust any equalizer band, the preset selection automatically switches to "Custom". This indicates that your current EQ settings no longer match any saved preset and are your own custom configuration.

**Saving Custom Presets:**
1. Adjust the equalizer bands to your desired settings (on the Equalizer page or by modifying any preset).
2. Navigate to the **Presets** page.
3. Enter a name for your preset in the text field at the top.
4. Click the **Save Preset** button to store your custom preset.

**Managing Custom Presets:**
- Custom presets appear alongside the built-in presets in the dropdown list.
- You can overwrite an existing custom preset by saving with the same name.
- Delete custom presets using the Delete Preset button (built-in presets cannot be deleted).
- Export and import presets to share or backup your configurations.
- Add optional descriptions and tags to organize your preset collection.
- Maximum of 50 custom presets can be saved.

### **Preset Modes**

WaveShaper offers three intelligent modes for automatic preset selection, accessible on the Presets page:

| Mode | Description |
|------|-------------|
| **Manual** | Full control over preset selection. Choose presets manually from the dropdown menu. Your selection persists until you change it. Ideal when you know exactly which EQ curve you want. |
| **Keyword** | Filename-based detection. WaveShaper analyzes the audio filename for genre keywords (e.g., "rock", "jazz", "vocal", "bass", "podcast") and automatically applies a matching preset when a file is loaded. Fast and lightweight. |
| **Analyze** | Intelligent FFT frequency analysis. When a file is loaded, WaveShaper performs real-time spectral analysis of the audio content and automatically selects the best-matching preset based on the actual sound characteristics. |

**Keyword Mode Keywords:**
Keyword mode recognizes the following words in filenames:
- `vocal`, `voice`, `speech` → **Vocal**
- `rock`, `metal` → **Rock**
- `jazz` → **Jazz**
- `classical`, `orchestra` → **Classical**
- `piano` → **Piano**
- `bass`, `hip`, `rap` → **Hip Hop**
- `podcast`, `interview` → **Podcast**
- `game`, `gaming` → **Gaming**
- `dance`, `club` → **Dance**
- `cinema`, `movie`, `film` → **Cinema**
- And more...

**How Analyze Mode Works:**

Analyze mode uses Fast Fourier Transform (FFT) analysis to understand the frequency content of your audio:

1. **Multi-Point Sampling:** Analyzes the frequency spectrum at multiple positions (10s, 30s, 60s) to get a representative sample of the entire track.
2. **6-Band Energy Analysis:** Calculates energy distribution across six frequency bands:
   - Sub-Bass & Bass (20-120 Hz)
   - Low-Mid / Warmth (120-400 Hz)
   - Mid / Vocals & Instruments (400-2500 Hz)
   - High-Mid / Presence (2500-5000 Hz)
   - Treble / Brilliance (5000-10000 Hz)
   - Presence / Air (10000+ Hz)
3. **Pattern Matching:** Compares the frequency profile against 30 preset characteristics to find the closest match.
4. **Automatic Application:** Applies the best-matching preset and updates the Active Preset display.

**Example Analyze Mode Detections:**
- Heavy sub-bass with warm low-mids → **Deep Bass** (e.g., dubstep, trap music)
- Strong mids with minimal highs → **Classical** or **Piano** (e.g., symphony, piano sonata)
- Full spectrum with presence in all bands → **Cinema** (e.g., movie soundtrack, orchestral score)
- Bass + highs with scooped mids → **Electronic** or **Dance** (e.g., EDM, house music)
- Speech-focused with clear mid-range → **Podcast** or **Spoken Word** (e.g., audiobook, interview)

## **Audio Effects Explained**

Beyond equalization, WaveShaper provides a comprehensive suite of audio effects that can transform your sound from subtle enhancement to dramatic creative manipulation. The Effects page is organized into four panels: Time Stretch, Reverb, Delay and Saturation.

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

### **Reverb and Space**

Reverb simulates the natural reflections of sound in physical spaces. When you clap your hands in a large hall, you hear the sound bounce off walls and decay over time. WaveShaper offers six reverb environments:

- **Room:** Small room ambience, subtle and natural
- **Hall:** Concert hall with longer decay for orchestral depth
- **Cathedral:** Very large space with extended reverb tail
- **Chamber:** Studio recording room simulation
- **Plate:** Classic studio reverb with smooth, dense decay
- **Spring:** Vintage spring reverb character

Each reverb type can be fine-tuned with five parameters:
- **Pre-Delay** (0–200 ms): The gap before reverb onset, creating a sense of distance
- **Decay Time**: How long the reverb tail lasts
- **Room Size**: How large the simulated space feels
- **HF Damping**: How quickly high frequencies decay, for natural or bright tails
- **Dry/Wet**: The balance between original and reverberant signal

### **Delay Effects**

Delay creates echoes by repeating the audio signal after a set time interval. WaveShaper provides six delay modes:

- **Simple:** Single repeat for basic echo effects
- **Ping-Pong:** Alternates between left and right speakers for spacious stereo effects
- **Multi-Tap:** Multiple delay times create rhythmic patterns
- **Filtered:** Delay with frequency filtering for darker, more vintage echoes
- **Stereo:** Independent delay times for each channel
- **Reverse:** Reversed delay trails for creative sound design

Delay parameters include **Delay Time** (up to 1000 ms) and **Feedback** (controls how many times the delay repeats).

### **Saturation**

Saturation adds harmonic distortion and warmth to your audio, emulating the pleasant characteristics of analog hardware. WaveShaper offers five saturation models:

- **Tape:** Warm, smooth saturation inspired by magnetic tape recorders
- **Tube:** Rich harmonic distortion with the character of vacuum tube amplifiers
- **Transistor:** Tighter, more aggressive clipping with solid-state character
- **Diode:** Asymmetric clipping for a raw, edgy distortion
- **Hard Clip:** Digital hard clipping for extreme distortion effects

Saturation parameters include **Drive Amount** (intensity of the effect), **Dry/Wet** (blend between clean and saturated signal) and **Output Gain** (compensate for volume changes).

### **Modulation**

Modulation effects add movement and animation to your audio by varying parameters over time using a low-frequency oscillator (LFO). WaveShaper provides six modulation types:

- **Tremolo:** Volume modulation creates a wavering, pulsing effect
- **Vibrato:** Pitch modulation adds subtle pitch variation for a natural, animated sound
- **Auto-Pan:** Stereo position sweeps left and right automatically for spatial movement
- **Chorus:** Multi-voice delay modulation creates a thick, ensemble-like sound
- **Phaser:** Allpass filter chain with LFO modulation for sweeping, jet-like tones
- **Flanger:** Short delay modulation produces metallic, swooshing effects

### **Creative Effects**

For more experimental sound design, WaveShaper includes seven creative effects:

- **Reverse:** Plays audio backwards for ambient textures and transitions
- **Stutter:** Creates rhythmic chopping effects by repeating short segments
- **Gate:** Cuts audio below a threshold for rhythmic silence patterns
- **Bitcrush:** Reduces bit depth for lo-fi, digital distortion character
- **Lo-Fi:** Degrades audio quality for vintage, nostalgic sound textures
- **Ring Mod:** Ring modulation produces metallic, bell-like tonal effects
- **Granular:** Breaks audio into tiny grains for textural, ambient manipulation

## **Dynamic Compression Guide**

### **What is Compression**

Dynamic compression is essential for controlling the volume differences in audio. Without compression, quiet parts might be too soft while loud parts distort or overpower the mix. A compressor automatically reduces the volume of signals that exceed a certain threshold, creating a more consistent and professional sound.

Think of compression like an automatic volume control that turns down the loud parts. This allows you to then raise the overall level, making quiet details more audible while preventing peaks from distorting.

### **Compression Presets**

Six purpose-built presets provide optimized starting points:

| Preset | Best For |
|--------|----------|
| **Vocal** | Spoken word, singing, podcasts |
| **Drums** | Drum loops, percussion, rhythmic material |
| **Bass** | Bass instruments, sub-heavy content |
| **Master** | Full mixes and mastering chains |
| **Gentle** | Subtle leveling without audible compression |
| **Custom** | Your own settings |

Each preset automatically configures the compressor parameters (threshold, ratio, attack, release, makeup gain and mix level) for the target material. You can further adjust any parameter after selecting a preset.

### **Compressor Controls**

The compressor provides precise control over dynamics processing:

- **Release** (Fast, Medium, Slow, Custom): How quickly compression disengages after the signal drops below threshold
- **Ratio** (1:1 to 20:1): The amount of gain reduction applied. Higher ratios mean more aggressive compression. Ratios above 10:1 approach limiting behavior.
- **Threshold** (-60 dB to 0 dB): The level above which compression begins. Lower thresholds compress more of the signal.
- **Attack** (1–500 ms): How quickly the compressor responds to signals exceeding the threshold
- **Makeup Gain** (0–24 dB): Compensates for the volume loss from compression
- **Parallel Mix** (0–100%): Blends compressed and uncompressed signals for parallel compression

**Additional Controls:**
- **Auto Makeup Gain:** Automatically compensates for gain reduction
- **Soft/Hard Knee:** Controls the transition curve at the threshold. Soft knee provides gradual onset, hard knee provides immediate compression.

### **Gate and Expander**

The Gate/Expander section removes unwanted noise and bleed from recordings by attenuating audio that falls below a set threshold:

- **Gate Threshold** (-80 dB to 0 dB): Audio below this level is attenuated
- **Range/Depth** (-80 dB to 0 dB): How much the signal is reduced when gated
- **Attack** (0–50 ms): How quickly the gate opens when signal exceeds threshold
- **Release** (10–500 ms): How quickly the gate closes after signal drops below threshold
- **Hold** (0–200 ms): Minimum time the gate stays open after triggering, preventing chattering on transients

## **Mastering Suite**

The Mastering page provides professional-grade tools for the final stage of audio production. It combines loudness metering, limiting, stereo imaging and analog-style effects into a cohesive mastering workflow.

### **Mastering Meter**

The mastering meter provides real-time monitoring across three display modes:

- **Peak / LUFS:** Displays left and right channel peak levels alongside integrated LUFS (Loudness Units Full Scale) measurement for broadcast-standard loudness monitoring
- **True Peak:** Shows inter-sample peak levels that may exceed 0 dBFS in the digital domain, critical for streaming and broadcast compliance
- **Loudness:** Dedicated LUFS display with loudness range (LRA) analysis

The meter shows separate bars for Left (L), Right (R) and Integrated (I) measurements with tooltips displaying precise dB values on hover.

### **Mastering Presets**

Six mastering presets provide industry-standard starting points:

| Preset | Target | Best For |
|--------|--------|----------|
| **Streaming** | -14 LUFS | Spotify, Apple Music, YouTube |
| **Broadcast** | -23 LUFS | TV, radio, podcast distribution |
| **Loud Master** | -8 LUFS | Competitive loudness for EDM, pop |
| **CD Master** | -12 LUFS | Physical CD distribution |
| **Vinyl** | -16 LUFS | Warm vinyl-style mastering |
| **Custom** | Adjustable | Your own target loudness |

Each preset configures **Target Loudness** (-24 to -6 LUFS) and **Output Gain** (-12 to +12 dB) for the selected delivery format.

### **Limiter**

The brick-wall limiter prevents audio from exceeding a set ceiling, ensuring clean output without digital clipping:

- **Lookahead** (1, 2, 5 or 10 ms): Anticipates peaks for transparent limiting. Longer lookahead catches more peaks but adds latency.
- **Ceiling** (-30 to 0 dB): Maximum output level. Set to -1 dB or lower for safe headroom.
- **Release** (10–500 ms): How quickly the limiter disengages after peak reduction

**Limiter Options:**
- **True Peak:** Enables inter-sample peak detection for accurate limiting
- **Auto Release:** Dynamically adjusts release time based on program material
- **Link Stereo:** Links left and right channel limiting to preserve stereo image

### **Stereo and Effects**

The Stereo & Effects panel provides mastering-grade stereo and analog processing:

**Stereo Mode and Width:**
- **Mono / Narrow / Normal / Wide / Extra Wide:** Quick stereo width presets
- **Width** (0–200%): Precise stereo width control from full mono (0%) to double-wide (200%)
- **Mid/Side** (-100 to +100): Balance between center (mid) and side content. Positive values emphasize sides for wider imaging, negative values emphasize center for focused mono content.

**Analog Effects:**
- **Exciter** (0–100%): Adds harmonic overtones and high-frequency sparkle for presence and air
- **Tape Saturation** (0–100%): Emulates the warm compression and harmonic richness of analog tape machines

## **Visualization and Monitoring**

### **Spectrum Analyzer**

The real-time spectrum analyzer displays the frequency content of your audio, helping you identify problematic frequencies, verify EQ adjustments and ensure a balanced mix.

**Display Modes:**
- **Linear:** Equal spacing across frequencies
- **Logarithmic:** More resolution in lower frequencies (matches human hearing perception)
- **Smooth:** Averaged display for easier reading
- **Peak:** Shows maximum values with decay
- **RMS:** Shows average energy levels
- **Octave:** Groups frequencies into octave bands for simplified analysis
- **Avg Hold:** Displays running averages with peak hold indicators

### **Activity Dashboard**

The Dashboard tracks your usage patterns and provides an overview of your audio processing activities. It includes user activity charts, account information, workspace analysis and recent project history with quick-access context menus for playback, file location and favorites.

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

The Player page provides comprehensive audio playback with real-time visualization, multiple playback modes, audio enhancement and full transport controls.

### **Playback Modes**

Five playback modes control how tracks are sequenced:

- **Normal:** Plays tracks in library order
- **Shuffle:** Randomizes playback order
- **Repeat One:** Continuously loops the current track
- **Repeat All:** Loops through all tracks in the library
- **Smart Mix:** Intelligent sequencing that considers audio characteristics

### **Audio Modes**

Five audio processing modes enhance playback for different listening scenarios:

- **Standard:** Clean, unprocessed output for reference listening
- **Night Mode:** Reduces dynamic range and limits volume for quiet environments
- **3D Audio:** Spatial audio enhancement for headphone listening with virtual surround
- **Cinema:** Full spectrum enhancement with spacious staging for movie-like immersion
- **Concert:** Live concert simulation with room ambience and crowd energy

A **Mono Check** toggle collapses stereo to mono, allowing you to verify stereo compatibility of your mix.

### **Player Controls**

- **Volume:** Master output volume with trackbar control (0–100%)
- **Stereo Balance:** Adjust left/right balance (-100 to +100)
- **Loop Mode:** Automatically repeat the current track once playback finishes
- **Crossfade:** Smooth transition between tracks (Off, Short 1s, Medium 3s, Long 5s)
- **Dynamic Range:** Compressed (Narrow), Normal, Wide or Extreme dynamic range for playback
- **Transport:** Play, Stop, Previous and Next buttons for full playback control

## **Preset Management**

The Presets page provides advanced tools for organizing, comparing and managing your EQ presets beyond basic save and load functionality.

### **A/B Comparison**

Compare two preset configurations side-by-side during playback:

1. **Capture A / Capture B:** Snapshot the current EQ state into slot A or B.
2. **Toggle A / B:** Instantly switch between the two captured states.
3. **Bypass:** Temporarily disable all EQ to compare with the unprocessed signal.
4. **Swap A↔B:** Exchange the contents of both slots.

This is essential for making informed mixing decisions by directly comparing different EQ approaches in real-time.

### **Preset Categories**

Advanced preset management features include:

- **Transition Mode:** Control how presets crossfade (Smooth, Instant or Crossfade)
- **Preset Quality:** Processing quality level (Basic, Standard, High, Ultra)
- **Complexity:** Adjust the processing complexity for the selected preset
- **Preset Morph (A/B):** Smoothly blend between two presets by sliding between them

## **Configuring Audio Settings**

The Settings page provides comprehensive control over audio processing, engine configuration and export parameters.

### **General Settings**

- **Startup View:** Choose which page opens when WaveShaper launches (Dashboard, Equalizer, Projects, Player, Effects, Compress, Presets or Settings)
- **Audio Mode:** Global audio channel mode (Stereo, Mono or Surround)
- **Sample Rate:** Playback sample rate selection (44 kHz, 48 kHz, 88 kHz, 96 kHz, 176 kHz, 192 kHz)
- **Bit Depth:** Audio processing bit depth (16 Bit, 24 Bit, 32 Bit)
- **Latency Mode:** Balance between responsiveness and stability (Low, Normal, High)
- **Dithering Type:** Algorithm for reducing quantization artifacts when lowering bit depth:
  - None, RPDF (Rectangular), TPDF (Triangular), TPDF + High-pass, Noise Shaping 1 (Gentle), Noise Shaping 2 (Medium), Noise Shaping 3 (POW-r style)
- **Dithering:** Toggle dithering noise application when reducing bit depth
- **Global Bypass:** Temporarily disable all EQ, compression and audio effects for A/B comparison

### **Processing Settings**

- **Real-Time Processing:** Toggle instant audio effect processing during playback for immediate feedback
- **Audio Quality:** Processing quality level (Low/Fast, Medium, High/Best, Ultra)
- **DSP Threads:** Number of processing threads (1–10) for parallel audio computation

### **Audio Engine**

- **Audio Driver:** Output driver selection (WASAPI Shared, WASAPI Exclusive, DirectSound)
- **Buffer Size:** Audio buffer size in samples (64, 128, 256, 512, 1024, 2048). Smaller buffers reduce latency, larger buffers improve stability.

### **Audio Devices**

- **Input Device:** Select the audio input device for recording or monitoring
- **Output Device:** Select the audio output device for playback

### **Audio Export**

- **Normalization:** Output level normalization (Off, Peak -1 dB, LUFS -14 Streaming, LUFS -16 Apple, LUFS -23 Broadcast)
- **Audio Quality:** MP3 bitrate selection (320, 256, 160, 128, 96, 64, 48, 32 kbps)
- **Export Format:** Output file format (WAV, FLAC, MP3, AAC, OGG)

Settings can be saved, imported from file, exported to file or reset to defaults using the action buttons.

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
2. Add space with reverb by selecting a room type and adjusting pre-delay, decay, room size and damping.
3. Create echoes with delay by choosing a mode and setting time and feedback.
4. Add warmth with saturation by selecting a model and dialing in the drive amount.
5. Experiment with time stretching, modulation and creative effects.

### **Step 4: Control Dynamics with Compression**

1. Go to the **Compress** tab.
2. Select a preset based on your material (Vocal, Drums, Bass, Master).
3. Fine-tune threshold and ratio for the amount of compression.
4. Adjust attack and release to shape transients.
5. Use the Gate/Expander to clean up noise between phrases.

### **Step 5: Master Your Audio**

1. Navigate to the **Mastering** tab.
2. Select a mastering preset matching your delivery target (Streaming, Broadcast, CD).
3. Enable the limiter and set the ceiling to prevent clipping.
4. Adjust stereo width and add exciter or tape saturation for character.
5. Monitor loudness levels on the mastering meter to meet platform standards.

### **Step 6: Export Your Processed Audio**

1. Return to the **Projects** tab.
2. Select your project and click **Export Project**.
3. Choose output format (`WAV`, `FLAC`, `MP3`, `AAC` or `OGG`).
4. Configure normalization and quality settings in Settings if needed.
5. Click **Export** and select your destination folder.

## **Customization**

### **Color Themes**

Personalize WaveShaper with seven color themes that completely transform the application's appearance. Each theme shifts the entire color palette including backgrounds, borders, accents and visualizations:

- **Ocean Blue** — Deep blue tones (default)
- **Forest Green** — Natural emerald greens
- **Sunset Orange** — Warm amber hues
- **Purple Night** — Rich amethyst purples
- **Cherry Blossom** — Soft rose and pink tones
- **Crimson Red** — Deep cherry reds
- **Phantom** — Bright cyan and teal

Changes apply immediately without restart.

### **Audio Quality and Performance**

Optimize WaveShaper for your hardware through the Settings page:

- **Audio Quality:** Choose from Low (Fast), Medium, High (Best) or Ultra processing quality
- **DSP Threads:** Allocate 1–10 processing threads based on your CPU capabilities
- **Buffer Size:** Adjust from 64 to 2048 samples to balance latency and stability
- **Audio Driver:** Select WASAPI Shared (compatible), WASAPI Exclusive (low-latency) or DirectSound

## **Updating Software**

WaveShaper includes automatic update functionality that checks for new versions on startup. When an update is available, it downloads the latest patch automatically and installs with minimal interruption. The application restarts with the new version after installation.

For manual updates or first-time installation, download the latest installer from the [Releases](https://github.com/BerndHagen/WaveShaper-Audio-Processor/releases) page and run it. The installer handles all dependencies and creates Start Menu and optional Desktop shortcuts.

## **Copyright**

This software is the intellectual property of the Author and is protected by international copyright laws.

1. **License:** You are granted a non-exclusive, non-transferable license to use the software for personal and commercial purposes.

2. **Modifications Prohibited:** Modification, decompiling, reverse-engineering or derivative work is prohibited without prior written consent.

3. **Attribution:** When redistributing, appropriate credit to the Author is required, including a link to the original source.

4. **Third-Party Libraries:** WaveShaper uses NAudio (MIT), NAudio.Lame (LGPL), SoundTouch.Net (LGPL), TagLibSharp (LGPL) and Newtonsoft.Json (MIT). Please review and comply with their respective licenses.

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
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-dashboard.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-dashboard.png" alt="WaveShaper Dashboard" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-equalizer.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-equalizer.png" alt="WaveShaper Equalizer" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Projects</th>
    <th>WaveShaper - Player</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-projects.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-projects.png" alt="WaveShaper Projects" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-player.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-player.png" alt="WaveShaper Player" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Effects</th>
    <th>WaveShaper - Mastering</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-effects.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-effects.png" alt="WaveShaper Effects" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-mastering.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-mastering.png" alt="WaveShaper Mastering" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Compressor</th>
    <th>WaveShaper - Presets</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-compressor.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-compressor.png" alt="WaveShaper Compressor" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-presets.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-presets.png" alt="WaveShaper Presets" width="450"></a></td>
  </tr>
  <tr>
    <th>WaveShaper - Settings</th>
    <th></th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-settings.png"><img src="https://github.com/BerndHagen/WaveShaper-Audio-Processor/raw/main/img/img_v2.0.0-waveshaper-settings.png" alt="WaveShaper Settings" width="450"></a></td>
    <td></td>
  </tr>
</table>
