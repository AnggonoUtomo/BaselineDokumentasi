# Katalog Module

| Module | Tujuan | Owns data | Kontrak Publik | Menerbitkan event | Mengonsumsi | dilarang dependensi | Pemilik |
|---|---|---|---|---|---|---|---|

## Boundary aturan

- module dilarang query module lain module's privat tabel secara langsung kecuali secara eksplisit disetujui.
- Lintas-module sinkron perilaku menggunakan eksplisit publik kontrak.
- Lintas-module asinkron perilaku menggunakan terdokumentasi events/messages.
- Shared kode wajib minimal dan dilarang memuat spesifik module aturan bisnis.

## Per-module template

### `<Module name>`

- Tujuan:
- Dalam scope:
- Di luar scope:
- Entities/aggregates:
- Publik aplikasi kontrak:
- event diterbitkan:
- event dikonsumsi:
- data ownership:
- Authorization boundary:
- dependensi:
- Invariants:
