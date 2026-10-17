# Sebklaey Web-Modelle

Gewichte für die Sebklaey-App-Demo. **CC BY-NC-SA 4.0 — keine kommerzielle Nutzung.**

## momo-llm/

Momos eigenes Saiten-Sprachmodell (Saiten-Transformer, 35,8 Mio Gewichte, int8+fp16, ~36 MB).
Läuft vollständig im Browser des Nutzers (Web Worker, WASM-frei) — keine Daten verlassen das Gerät.

- `momo-llm.bin` — Gewichte (int8 mit absmax-Skalen pro Tensor + fp16 für kleine Tensoren)
- `momo-llm.json` — Manifest (Konfig, Tensordeskriptoren, Offsets in Bytes)
- `momo-vocab.json` — BPE-Vokabular (SentencePiece-kompatibel, user-defined `DU:`/`MOMO:`/`<|ende|>`, byte_fallback)
