# ShadersMod & Culling Optimizer (MCPE / Helio G99)

Paket optimasi visual dan performa khusus untuk **Minecraft Bedrock (MagicLoader)** di chipset **MediaTek Helio G99 (GPU Mali-G57 MC2)**.

---

## 🚀 1. Addon Culling Optimizer (Render Depan Kamera Saja)
- **File**: `HelioG99-CullingOptimizer.mcpack`
- **Download Langsung**: [Unduh HelioG99-CullingOptimizer.mcpack](https://raw.githubusercontent.com/KyokoApp/ShadersMod/main/HelioG99-CullingOptimizer.mcpack)
- **Cara Kerja (Frustum & Occlusion Culling)**:
  - Blok, pohon, partikel, dan mob yang berada **di belakang punggung pemain dipotong total (0% render)**.
  - Gua bawah tanah yang tertutup dinding batu tebal tidak dihitung geometri bayangannya.
  - **Efek**: GPU Mali-G57 hanya fokus merender apa yang tertangkap di layar HP kamu. FPS melonjak drastis tanpa menurunkan kualitas visual sedikit pun.
- **Cara Pasang**:
  - Download file `.mcpack` di atas.
  - Klik/buka file tersebut menggunakan Minecraft Bedrock -> Otomatis terimport.
  - Masuk ke **Settings** -> **Global Resources** -> Aktifkan `HelioG99 Camera Culling Optimizer`.

---

## 🌟 2. Shader BSL MaxTurbo (Frustum Culling Edition)
- **File**: `BSL-60FPS-MaxTurbo.zip`
- **Download Langsung**: [Unduh BSL-60FPS-MaxTurbo.zip](https://raw.githubusercontent.com/KyokoApp/ShadersMod/main/BSL-60FPS-MaxTurbo.zip)
- **Kombinasi Sempurna**:
  - Shader BSL sudah diinject flag `frustum.culling = true`, `shadow.culling = true`, dan `occlusion.culling = true`.
  - Air realistis bergelombang, warna sinematik BSL, dan goyangan dedaunan tetap 100% utuh di depan pandangan mata.
