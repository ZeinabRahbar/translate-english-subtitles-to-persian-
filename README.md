# SRT Subtitle Translator (English to Persian)

A Python-based utility designed to automate the translation of subtitle files (`.srt`) into Persian while strictly maintaining the original timing and structure.

## 🚀 Features
* **Format Preservation:** Keeps subtitle indices and timestamps (`00:00:00,000 --> 00:00:00,000`) intact.
* **Batch Translation:** Processes entire SRT files line-by-line automatically.
* **Error Resilience:** Includes `try-except` blocks to handle translation API errors, ensuring the script doesn't crash on problematic lines.
* **Real-time Console Output:** Displays translated blocks in the console during the process for live monitoring.
* **Automatic Export:** Saves the final translated content directly to an `output.srt` file encoded in UTF-8.

## 🛠️ Requirements
* Python 3
* A translation library (e.g., `googletrans` or similar)
* Jupyter Notebook or Google Colab

## 📖 How It Works
1. **Parsing:** The script reads the source SRT file and identifies the index, time range, and text components.
2. **Translation:** The text component is sent to the translation engine to be converted into Persian.
3. **Reconstruction:** The script reassembles the components into the standard SRT format.
4. **Saving:** The result is written to `output.srt`.

## 🖥️ Usage
1. Open `final_translate_sub.ipynb` in your preferred notebook editor.
2. Upload or specify the path to your English SRT file.
3. Run the cells.
4. Download the generated `output.srt` from the local directory.

## ✨ Fun Fact
This project was born out of pure K-Drama impatience! Instead of waiting days for official Persian fan-subs to be released, I wrote this code so I could translate English subs instantly and watch the latest episodes before anyone else.

## ⚠️ Notes
* **Encoding:** The script uses `utf-8` encoding to ensure Persian characters are displayed correctly.
* **Context:** Automated translation may require manual proofreading for cultural nuances or gender-specific grammar in Persian.
