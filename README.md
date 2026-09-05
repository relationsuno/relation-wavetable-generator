# 3D Wavetable & UHM Studio

[English](#english) | [日本語](#japanese)

---

<a name="english"></a>
## English

A browser-based interactive 3D wavetable generator and synthesizer. Draw custom waveforms and terrains directly on a 2D canvas, visualize the full XYZ 3D wavetable mesh in real time, audition with the built-in Web Audio synth engine, and export ready-to-use **`.wav`** files (optimized for SUNO Studio 2.0, Xfer Serum, Vital, Pigments) and **`.uhm`** scripts (for u-he Hive).

### 🌟 Key Features

- **Interactive 2D Terrain / Wave Painter**:
  - Draw waveform contours directly. Left-click for positive peaks (mountains), right-click or Shift-drag for negative valleys.
  - Quick utility tools: Invert, Smooth, and Clear.
- **Real-Time 3D Wireframe Visualizer (XYZ Axes)**:
  - **X-axis**: Phase / Cycle (0 to 2048 samples).
  - **Y-axis**: Frame / Wavetable Position (Depth).
  - **Z-axis**: Amplitude (-1.0 to +1.0).
  - Matches the exact 3D wireframe style of **SUNO Studio 2.0** and modern wavetable synths.
  - Free mouse-drag 3D rotation with a glowing white active playhead line.
- **Real-Time Audio Preview (Web Audio API)**:
  - Audition the wavetable instantly in your browser with looping playback.
  - Automatic bidirectional LFO sweep across wavetable frames with adjustable speed (0.25 Hz to 2.0 Hz).
  - Pitch selector (C2 Bass, C3 Mid, C4 Lead).
- **Non-Linear Sound Modulation (FX Engine)**:
  - **Wavefolder**: Buchla/West-Coast style wavefolding for aggressive, rich overtones.
  - **FM Sweep**: Dynamic frequency/phase modulation scaling with frame position.
  - **Hard Sync**: Aggressive oscillator sync windowing for cutting leads.
  - **Vocal Resonator**: Formant filter resonances (vowel-like timbres).
  - **Warm Overdrive**: Smooth hyperbolic tangent (`tanh`) saturation.
- **Customizable Frame Lengths (WAV Duration)**:
  - **32 Frames (~1.5s)**: ★ Optimal for **SUNO Studio 2.0** (clean, crisp, uncluttered 3D view).
  - **64 Frames (~3.0s)**: Standard balanced duration.
  - **128 Frames (~6.0s)**: Long evolving pads.
  - **256 Frames (~11.9s)**: Maximum resolution (Serum full-table standard).
- **Zero Dependencies**:
  - Standalone single-file application (`index.html`). No build step, no npm, works offline.

### 🎛️ Compatible Synthesizers

- **SUNO Studio 2.0**: Native Wavetable Synth (`.wav`, 32 frames recommended).
- **Xfer Records Serum**: Standard wavetable format (`.wav`).
- **Matt Tytel Vital**: Full wavetable import (`.wav`).
- **u-he Hive / Hive 2**: Native mathematical wavetable language (`.uhm`).
- **Arturia Pigments, Korg modwave, Ableton Wavetable**, etc.

### 🚀 Getting Started

1. Clone or download this repository.
2. Open `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Select a preset (e.g., *SUNO Metallic Spike*) or paint your own terrain on the 2D canvas.
4. Click **"試聴 (Play Sound)"** to hear the morphing wavetable.
5. Click **"🎵 .wav をダウンロード"** or **"📄 .uhm をダウンロード"** to export.
6. Drag & drop the `.wav` file into SUNO Studio 2.0 or your synth of choice!

---

<a name="japanese"></a>
## 日本語

ブラウザ上で直感的に波形を描き、**3Dウェーブテーブル（XYZ軸）** をリアルタイムプレビュー＆試聴しながら、**WAVファイル**（SUNO Studio 2.0、Serum、Vital等に対応）および **UHMスクリプト**（u-he Hive対応）を生成できるWebツールです。

### 🌟 主な機能

- **直感的な2D波形・地形ペインター**:
  - マウスで直感的に波形の山と谷を描画（左ドラッグ：正の振幅、右ドラッグ/Shift：負の振幅）。
  - 「反転」「平滑化」「クリア」の補助ツール完備。
- **SUNO Studio 2.0スタイルのリアルタイム3Dビジュアライザー**:
  - **X軸（横）**: 位相・波形1周期（0〜2048サンプル）
  - **Y軸（奥行き）**: フレーム・Wavetable Position（時間変化）
  - **Z軸（縦）**: 振幅（-1.0 〜 +1.0）
  - マウスドラッグで3D視点を自由に回転可能。現在発音中のフレームが白いネオンラインで光ります。
- **Web Audio APIによるリアルタイム音色試聴**:
  - ブラウザ上で即座にシンセサイザーとして発音・試聴可能。
  - LFO自動スキャン機能により、奥から手前へフレームが連続往復するダイナミックな音色変化を耳で確認できます。
  - 基音切り替え（C2低音 / C3中音 / C4高音）。
- **劇的な音色変化を生む非線形モジュレーション (FX)**:
  - **Wavefolder**: 波形を限界値で折り返し、強烈で過激な倍音を生成（西海岸シンセ風）。
  - **FM Sweep**: フレーム進行とともに金属的な唸りを付加する周波数変調。
  - **Hard Sync**: 急峻な倍音を生むオシレーター・シンク。
  - **Vocal Resonator**: 人間の声のような母音共鳴（フォルマント）。
  - **Warm Overdrive**: 温かみのあるアナログ風サチュレーション。
- **SUNOに最適化されたフレーム数（WAVの長さ）切り替え**:
  - **32 フレーム (約 1.5 秒)**: ★ **SUNO Studio 2.0 最適**（波形同士が重ならずクッキリ美しく表示されます）。
  - **64 フレーム (約 3.0 秒)**: バランスの良い標準長。
  - **128 フレーム (約 6.0 秒)**: ゆっくり移り変わるパッド向け。
  - **256 フレーム (約 11.9 秒)**: 従来のSerum最大サイズ。
- **完全スタンドアロン & 外部依存なし**:
  - `index.html` 1ファイルのみで動作。インストーラーやnpm、外部CDN不要で、オフラインでも即座に起動します。

### 🎛️ 対応シンセサイザー

- **SUNO Studio 2.0**: Wavetable Oscillator A/B（`.wav`、32フレーム推奨）
- **Xfer Records Serum**（`.wav`）
- **Matt Tytel Vital**（`.wav`）
- **u-he Hive / Hive 2**（`.uhm` スクリプト直接読み込み）
- **Arturia Pigments / Korg modwave / Ableton Wavetable** など

### 🚀 使い方

1. このリポジトリをダウンロード（またはクローン）します。
2. `index.html` をブラウザ（Chrome, Edge, Safari等）でダブルクリックして開きます。
3. プリセット（「SUNO Metallic Spike」など）を選ぶか、左のキャンバスに自由に波形を描きます。
4. **「試聴 (Play Sound)」** を押して音を確認し、FXやフレーム数を好みに調整します。
5. **「🎵 .wav をダウンロード (SUNO用)」** または **「📄 .uhm をダウンロード」** をクリックします。
6. ダウンロードされた `.wav` を SUNO Studio 2.0 の Oscillator に読み込んで演奏をお楽しみください！

---

### 📄 License

MIT License
