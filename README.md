# BOOKITCA Voice

Frozen model files for **BOOKITCA Voice**, the on-device read aloud voice in the
[BOOKITCA](https://bookitca.app) app for iPhone and iPad. The app downloads them from the
release `supertonic-3-int8-v1` and checks every file against the SHA-256 below.

## What is inside

Supertonic 3 by Supertone Inc. (31 languages, 44.1 kHz, ten voice styles).
The original project has been archived; this repository keeps the exact version BOOKITCA uses.

- `duration_predictor.int8.onnx`, `text_encoder.int8.onnx`, `vector_estimator.int8.onnx`,
  `vocoder.int8.onnx`: int8 quantized by the sherpa-onnx project (k2-fsa,
  `sherpa-onnx-supertonic-3-tts-int8-2026-05-11`).
- `tts.json`, `unicode_indexer.json`, `F1.json` to `F5.json`, `M1.json` to `M5.json`: unmodified,
  from Hugging Face `supertone-oss-archive/supertonic-3`, revision `aafc6e32416a594460b32413efc49d7fe4ce6d46`.

**Notice of modification:** the four `.onnx` files are int8 quantized copies of the original
weights. Nothing else was changed.

## License

The model is licensed under the **BigScience Open RAIL-M License** (see `LICENSE`).
Its use-based restrictions (paragraph 5 and Attachment A) apply to everyone who uses the model,
including users of BOOKITCA. Among other things, the model must not be used to break the law,
to impersonate others without their consent, to spread false information meant to harm,
or to harass others.

The Supertonic inference code is MIT licensed, Copyright (c) 2025 Supertone Inc.

## Checksums (SHA-256)

| File | Bytes | SHA-256 |
|---|---:|---|
| `F1.json` | 292046 | `bbdec6ee00231c2c742ad05483df5334cab3b52fda3ba38e6a07059c4563dbc2` |
| `F2.json` | 292423 | `7c722c6a72707b1a77f035d67f0d1351ba187738e06f7683e8c72b1df3477fc6` |
| `F3.json` | 290794 | `12f6ef2573baa2defa1128069cb59f203e3ab67c92af77b42df8a0e3a2f7c6ab` |
| `F4.json` | 291808 | `c2fa764c1225a76dfc3e2c73e8aa4f70d9ee48793860eb34c295fff01c2e032b` |
| `F5.json` | 291479 | `45966e73316415626cf41a7d1c6f3b4c70dbc1ba2bee5c1978ef0ce33244fc8d` |
| `M1.json` | 291748 | `e35604687f5d23694b8e91593a93eec0e4eca6c0b02bb8ed69139ab2ea6b0a5b` |
| `M2.json` | 292055 | `b76cbf62bac707c710cf0ae5aba5e31eea1a6339a9734bfae33ab98499534a50` |
| `M3.json` | 290198 | `ea1ac35ccb91b0d7ecad533a2fbd0eec10c91513d8951e3b25fbba99954e159b` |
| `M4.json` | 291522 | `ca8eefad4fcd989c9379032ff3e50738adc547eeb5e221b82593a6d7b3bac303` |
| `M5.json` | 291469 | `dd22b92740314321f8ae11c5e87f8dd60d060f15dd3a632b5adf77f471f77af2` |
| `duration_predictor.int8.onnx` | 3700147 | `c3eb91414d5ff8a7a239b7fe9e34e7e2bf8a8140d8375ffb14718b1c639325db` |
| `text_encoder.int8.onnx` | 36416150 | `c7befd5ea8c3119769e8a6c1486c4edc6a3bc8365c67621c881bbb774b9902ff` |
| `tts.json` | 8253 | `42078d3aef1cd43ab43021f3c54f47d2d75ceb4e75f627f118890128b06a0d09` |
| `unicode_indexer.json` | 277676 | `9bf7346e43883a81f8645c81224f786d43c5b57f3641f6e7671a7d6c493cb24f` |
| `vector_estimator.int8.onnx` | 78400833 | `20cd86fa5c6effedfda0e7cffe5b0569ca401c440a0c3a1d72bf39286c0db3fd` |
| `vocoder.int8.onnx` | 25991073 | `e923d60f53f95eb1ce235f1dc33ec56d9c057823c96fa6f8acf98f32b0da6152` |
