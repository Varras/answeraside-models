# AnswerAside speech model files

The [AnswerAside](https://answeraside.com) desktop app transcribes calls on the user's PC. On first use it downloads these model files from this repository's Releases, checks each one against a pinned SHA-256, and keeps them in `%APPDATA%\AnswerAside\models`. Audio never leaves the PC.

This repository holds only redistributed model files and their licenses. No app code.

## Release `speech-model-v1`

| File | SHA-256 | From |
| --- | --- | --- |
| `config.json` | `666903c76b9798caf2c210afd4f6cd60b08a8dbf9800ec8d7a3bc0d2148ac466` | Parakeet |
| `vocab.txt` | `d58544679ea4bc6ac563d1f545eb7d474bd6cfa467f0a6e2c1dc1c7d37e3c35d` | Parakeet |
| `nemo128.onnx` | `a9fde1486ebfcc08f328d75ad4610c67835fea58c73ba57e3209a6f6cf019e9f` | Parakeet |
| `encoder-model.int8.onnx` | `6139d2fa7e1b086097b277c7149725edbab89cc7c7ae64b23c741be4055aff09` | Parakeet |
| `decoder_joint-model.int8.onnx` | `eea7483ee3d1a30375daedc8ed83e3960c91b098812127a0d99d1c8977667a70` | Parakeet |
| `silero_vad.onnx` | `1a153a22f4509e292a94e67d6f9b85e8deb25b4988682b7e174c65279d8788e3` | Silero VAD |

The files are byte-for-byte copies of their sources; nothing was changed here.

## Credits and licenses

- **Parakeet TDT 0.6B v3** by NVIDIA ([nvidia/parakeet-tdt-0.6b-v3](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3)), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Converted to ONNX and quantized to int8 by istupakov ([istupakov/parakeet-tdt-0.6b-v3-onnx](https://huggingface.co/istupakov/parakeet-tdt-0.6b-v3-onnx), revision `8f23f0c03c8761650bdb5b40aaf3e40d2c15f1ce`). See `LICENSE-parakeet.txt`.
- **Silero VAD v6.2.2** by the Silero Team ([snakers4/silero-vad](https://github.com/snakers4/silero-vad), tag `v6.2.2`), MIT License. See `LICENSE-silero-vad.txt`.
