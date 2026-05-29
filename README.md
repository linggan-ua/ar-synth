# AR Synth Workstation

AR 合成器工作站 —— 基于 WebAR 的虚拟合成器与鼓机演奏平台。

对准合成器卡或鼓机卡，即可在 AR 中看到 3D 合成器/鼓机界面，直接触摸演奏。

## 技术栈

- **A-Frame + AR.js** — 稳定的 AR 标记识别与跟踪
- **Three.js** — 程序化 3D 合成器/鼓机建模
- **Web Audio API** — 实时音频合成引擎

## 功能

### 合成器
- 25 键触控键盘
- 4 种预设模式：SYNTH / GUITAR / BASS / DRUM
- 3 种波形：Saw / Square / Sine
- ADSR 包络推子 + Filter (Cutoff / Resonance)
- FX 效果 (Delay)
- Glide / Arp / Hold 演奏模式
- Pitch Bend + Modulation 触控条
- 双指缩放

### 鼓机
- 8 打击垫：Kick / Snare / Clap / Rim / Hi-Hat / Open Hat / Tom / Crash
- 5 控制旋钮：Tone / Decay / Drive / Space / Level
- 内置节奏模板 (Play / Stop)
- 键盘鼓机映射

## 使用方式

1. 打开页面，点击"启动 AR 体验"
2. 允许摄像头权限
3. 将识别卡对准摄像头
   - **合成器卡** → 显示 AR Mini Synth Workstation
   - **鼓机卡** → 显示 QR Drum Machine
4. 触摸 3D 界面演奏

## 本地运行

```bash
# 启动本地服务器（需要 HTTPS）
npx http-server -p 8080 -S -C cert.pem
```

> WebAR 需要 HTTPS 或 localhost 才能访问摄像头。

## License

MIT
