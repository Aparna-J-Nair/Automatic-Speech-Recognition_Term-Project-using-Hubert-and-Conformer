# Conformer Speech Recognition

This project demonstrates how to build and evaluate a speech-to-text system using state-of-the-art transformer-based models (e.g., HuBERT, Wav2Vec2, Conformer) with Hugging Face’s transformers library and ESPnet’s pretrained models.

## Features:

- Pretrained ASR models (Wav2Vec2Processor, HubertForCTC, Speech2Text).

- Support for loading datasets with Hugging Face datasets.

- Audio preprocessing and text normalization.

- End-to-end transcription pipeline for speech recognition.

- Can be run in Google Colab with Drive integration.

Requirements

The notebook requires the following dependencies:

```python
pip install transformers datasets soundfile espnet_model_zoo
```

### Additional common packages:

- numpy

- string

If running on Colab, Google Drive integration is included.

### Usage

1. Open the notebook: Conformer.ipynb.

2. Mount your Google Drive (if on Colab) to access datasets and save outputs.

3. Load your dataset or audio files.

4. Run the preprocessing functions:

    - text_normalizer(text) → cleans and normalizes transcriptions.

    - map_to_array(batch) → converts audio files to numpy arrays.

5. Choose a pretrained model (HuBERT, Wav2Vec2, Conformer) and run inference.

### File Structure

- Conformer.ipynb → Main Jupyter Notebook for ASR pipeline. (Please download the zip to use it)

7. Evaluate transcription quality using metrics (e.g., WER/CER).
