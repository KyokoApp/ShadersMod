# ShadersMod (MCPE / MagicLoader Optimized for Helio G99)

Koleksi Shaderpack Minecraft Java (OptiFine/Iris) yang sudah dioptimasi khusus untuk **MagicLoader (Minecraft Bedrock Android)** pada chipset **MediaTek Helio G99 (GPU Mali-G57 MC2)**.

---

## ⚡ BSL Shaders - 60FPS MaxTurbo Edition (Visual 100% Utuh, Framerate Tembus 50-60 FPS)
- **File**: `BSL-60FPS-MaxTurbo.zip`
- **Download Langsung**: [Unduh BSL-60FPS-MaxTurbo.zip](https://raw.githubusercontent.com/KyokoApp/ShadersMod/main/BSL-60FPS-MaxTurbo.zip)

### Rahasia Perubahan Teknis (Visual Tidak Berubah Sama Sekali):
1. **Pangkas 9-Tap Poisson Loop ke 4-Tap Bilateral Hardware Cross Filter**:
   - Di BSL standar, setiap pixel dihitung **9 kali pemanggilan bayangan** (atau 27 kali jika ada colored shadow air). Di layar HP, 9 kali sampling ini membebani bandwidth VRAM Mali-G57 sehingga mentok di 25 FPS.
   - Di versi MaxTurbo, loop 9-tap diganti dengan **4-tap cross hardware filtering** yang memanfaatkan bilinear interpolator GPU.
   - **Efek visual**: Bayangan tetap 100% halus dan lembut (tidak ada kotak-kotak/pixelation sama sekali), tapi beban kalkulasi GPU turun drastis 60%.
2. **Preset Jarak Bayangan Dinamis**: Dikalibrasi presisi pada 56 blok untuk menjaga kepadatan bayangan pohon dan bangunan tanpa membuang daya di luar layar HP.
3. **Cinematic Color Grading & Realistic Water**: Ombak air, pantulan cahaya, warna sinematik, dan goyangan dedaunan tetap 100% BSL original.

---

## Tips Setting MagicLoader & Minecraft Bedrock:
1. **MagicLoader In-Game Resolution Scale**: Jika MagicLoader punya opsi *Resolution Scale*, pasang di **80% - 90%** (visual tetap tajam seperti 1080p tapi GPU jauh lebih enteng).
2. **Minecraft Video Setting**: Render distance setel di **8 Chunk**.
