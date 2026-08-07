# Strategi Pengujian

## tujuan

## pengujian levels

| tingkat | Tujuan | Ruang Lingkup | Tool | wajib di CI |
|---|---|---|---|---|

## pengujian selection aturan

- bisnis aturan memerlukan focused unit/domain pengujian ketika appropriate.
- Publik perilaku memerlukan integrasi/feature pengujian.
- bug perbaikan memerlukan failing regresi pengujian sebelum atau alongside perbaikan.
- kritis pengguna journeys memerlukan end-to-end coverage ketika feasible.

## pengujian data

## Isolation dan eksternal services

## keamanan pengujian

## performa pengujian

## kualitas gate

| gate | perintah/periksa | Blocking threshold |
|---|---|---|

## Flaky pengujian kebijakan

 tidak retry away unexplained kegagalan. catat pemilik, cause hypothesis, dan corrective task.

## Bukti format

```text
Command:
Result:
Relevant output:
Environment:
Date:
```
