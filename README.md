# akan-blind-denoising-data

Recordings for the `akan-blind-denoising` benchmark task, packed as one Python wheel so the task image can install them with a pinned SHA-256.

| File | Size | SHA-256 |
| --- | --- | --- |
| `akan_blind_denoising_data-1.0.0-py3-none-any.whl` (release v1.0.0) | 880,201,247 bytes | `1018221218a234884f0dbd03a70de2e4b24b377f534420940f5b5136ea882639` |
| `mixtures.flac` (inside the wheel) | 770,836,376 bytes | `55c258327c53b0b29edec0e3a499f7fda55fb35941e9a97ba34c6e3cf7c4e76f` |
| `hidden_assets.bin` (inside the wheel) | 109,363,100 bytes | `0ed98850d7d8721404fd9ee7565a6fdeb9b83acf0fedd3808be12e19fe4acd56` |

`mixtures.flac` is 10.9 hours of noisy 16 kHz speech: Akan speech pieces mixed with recorded noise. `hidden_assets.bin` is encrypted, and its key is not published here.

Install:

```
pip install --no-deps --require-hashes --target DIR "akan-blind-denoising-data @ https://github.com/prawalpokharel/akan-blind-denoising-data/releases/download/v1.0.0/akan_blind_denoising_data-1.0.0-py3-none-any.whl#sha256=1018221218a234884f0dbd03a70de2e4b24b377f534420940f5b5136ea882639"
```

## Sources and licence

- Speech: the Akan part of WAXAL ("WAXAL: A Large-Scale Multilingual African Language Speech Corpus", arXiv:2602.02734, Google Research), recorded by the University of Ghana and published as UGSpeechData, <https://doi.org/10.57760/sciencedb.22298>. Licence: Creative Commons Attribution 4.0 International. <https://huggingface.co/datasets/google/WaxalNLP>
- Noise: MUSAN ("MUSAN: A Music, Speech, and Noise Corpus", David Snyder, Guoguo Chen and Daniel Povey, 2015, arXiv:1510.08484), <https://www.openslr.org/17/>. Licence: Creative Commons Attribution 4.0 International.

The files here adapt both sources (cut into pieces, resampled to 16 kHz, mixed, rescaled and re-recorded in a room) and are released under Creative Commons Attribution 4.0 International.
