# AGM M7 firmware

Proprietary firmware for the AGM M7 (MT6739), used by the NixOS and LineageOS ports. See `LICENSE`.

| File | Use | SHA-256 |
|---|---|---|
| `rgx.fw.signed` | GE8100 GPU firmware (DDK 1.9), loaded as `powervr/rogue_22.49.21.16_ddk19.fw` | `35208dc3e488d2e8f7d768d4a96e118e0b4e87f8857d10c01ce65ba6da366d03` |
| `ROMv2_lm_patch_1_0_hdr.bin` | CONSYS ROM patch | `9e759e09f03e993aee6ab8aab19164f965df4789f2710fdb8f625802ea643645` |
| `ROMv2_lm_patch_1_1_hdr.bin` | CONSYS ROM patch | `194e2acb5aa185154d23ace9f0a6150393c2a972a3832e3eef5d22f10d5b45d9` |
| `WIFI_RAM_CODE_6755` | Wi-Fi firmware | `8d5e2913fa890def6f2c4398c61cc24f08f5731a60dd041b8fe8af5463f507e7` |
| `WMT_SOC.cfg` | WMT configuration | `f4b112fd042dd1025017e35998e25ec0befeb05cfe424f38bf27e3222299ce0d` |

LineageOS: check out as `vendor/agm/m7`; `device/agm/m7` inherits `m7-vendor.mk`.

NixOS: `nixos-agm-m7` uses this repo as a flake input (`flake = false`) and installs the files with `hardware.firmware`.
