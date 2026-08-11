# Nexus AI: The Intelligent Product Management Workspace

<div align="center">
  <!-- Ganti link gambar di bawah dengan logo asli Nexus AI jika ada -->
  <img src="https://via.placeholder.com/200x200.png?text=Nexus+AI+Logo" alt="Nexus AI Logo" width="200" height="200">
</div>

<!-- Profile Views -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=nexus-ai-org&style=flat-square&color=blue" alt="Profile views" />
</div>

## 📖 Deskripsi Proyek

**Nexus AI** adalah sistem manajemen produk komprehensif berbasis kecerdasan buatan (AI) yang dirancang untuk mempercepat alur kerja *Product Manager* dan tim *engineering*. Nexus memungkinkan pengguna untuk membuat, mengelola, dan mengotomatiskan pembuatan *Product Requirements Document* (PRD), serta menyediakan asisten AI (*Ask Nexus*) yang dapat menjawab pertanyaan spesifik berdasarkan konteks dokumen proyek (RAG).

### 🎯 Tujuan Utama
- Mempercepat siklus pembuatan dokumen spesifikasi produk (PRD).
- Menghilangkan miskomunikasi antar anggota tim (PM, Desainer, Engineer) melalui *Single Source of Truth*.
- Memudahkan pencarian informasi spesifik di lautan dokumen proyek menggunakan *Retrieval-Augmented Generation* (RAG).
- Menyediakan *workspace* terintegrasi (File, Folder, Tim) dalam satu *dashboard* modern.

## 🏗️ Arsitektur Sistem

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Frontend      │    │ Backend (Nexus)  │    │ Backend (AI)    │
│   (React +      │◄──►│ (Express.js +    │◄──►│ (Express.js +   │
│   Tailwind)     │    │  MongoDB)        │    │  Gemini API)    │
└─────────────────┘    └──────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│  Interactive UI │    │  Auth & Storage  │    │ RAG & Embeddings│
│  Real-time SSE  │    │  RBAC & Teams    │    │ PRD Generation  │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 🚀 Fitur Utama

### 🤖 Fitur Kecerdasan Buatan (AI)
- **AI PRD Generator**: Menghasilkan PRD lengkap dari *draft* dokumen acak atau *audio transcript* menggunakan Google Gemini.
- **Ask Nexus (RAG Copilot)**: Fitur *chat* AI yang paham 100% tentang konteks proyek Anda. Bertanya tentang spesifikasi proyek? AI akan menjawab beserta sitasi ke dokumen aslinya!
- **Clarification Wizard**: AI akan secara cerdas menanyakan detail-detail yang "kurang lengkap" dari *draft* Anda sebelum membuat PRD.

### 💻 Frontend
- **Interface Modern**: Dibangun dengan **React 18** dan **Tailwind CSS**.
- **UX Interaktif**: Mendukung *Drag & Drop* untuk manajemen *file* dan direktori.
- **Data Fetching Cepat**: Integrasi Axios yang sangat efisien untuk *seamless experience*.

### ⚙️ Backend & Infrastruktur
- **Microservices-ish**: Pemisahan antara *Core Service* (Manajemen Proyek, Autentikasi) dan *AI Service* (Generasi AI, *Text Embedding*).
- **Database Skalabel**: Menggunakan **MongoDB** untuk menyimpan *file metadata*, pengguna, tim, serta vektor *embedding* dokumen.
- **Secure Authentication**: Sistem OTP, reset *password*, dan JWT.

## 👥 Tim Pengembang

**Tim ID**: CC25-XXXXX *(isi dengan ID Tim)*  
**Tema**: *Productivity & Tooling*

| ID | Nama | Learning Path | Github |
|----|----- |---------------|--------| 
| MC222D5Y1282 | **Refa Muhammad** | Machine Learning / Backend Engineer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/RefaMuhammad) |
| XXXXXXXXXXXX | **[Nama Anggota 2]** | Front-End Developer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/[Username]) |
| XXXXXXXXXXXX | **[Nama Anggota 3]** | Back-End Developer | [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/[Username]) |
*(Tambahkan anggota tim lainnya di sini)*

## 🙏 Acknowledgments

- **Google Gemini API** untuk otak utama di balik fitur AI (*Ask Nexus* dan PRD *Generation*).
- **React & Tailwind Community** untuk ekosistem *frontend* yang luar biasa.
- **MongoDB** untuk solusi *database* yang fleksibel.
