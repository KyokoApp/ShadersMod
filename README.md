# ShadersMod & AI-SuperResolution (Helio G99 Mali-G57)

Optimasi shaderpack Minecraft khusus **MagicLoader Bedrock** pada chipset **MediaTek Helio G99**.

---

## ⚡ BSL Shaders - AI Turbo Edition (FSR Adaptive Reconstruction)
- **File**: `BSL-AI-Turbo-HelioG99.zip`
- **Download Langsung**: [Unduh BSL-AI-Turbo-HelioG99.zip](https://raw.githubusercontent.com/KyokoApp/ShadersMod/main/BSL-AI-Turbo-HelioG99.zip)

### Cara Kerja Teknik Mirip AI (FSR 1.0 CAS Sharpening):
1. **Pass-through Reconstruction (FSR CAS Sharpening Level 2)**:
   - Diaktifkan langsung di pass akhir post-processing (`final.glsl`).
   - Tepi blok, garis bayangan, ombak air, dan dedaunan dipertajam otomatis secara adaptif sesuai kontras layar.
2. **Kombinasi Penghemat Beban GPU**:
   - Jika resolusi layar HP atau render scale diturunkan sedikit (misal ke 80% di MagicLoader / setting resolusi), visual **tetap tampak tajam seperti 1080p native**, tetapi GPU Mali-G57 bekerja jauh lebih ringan sehingga framerate bisa melesat menuju 60 FPS.
3. **Preservasi Efek 100%**:
   - Bayangan lembut BSL, ombak air jernih dengan pantulan matahari, goyangan dedaunan, dan warna sinematik tetap 100% aktif utuh.
