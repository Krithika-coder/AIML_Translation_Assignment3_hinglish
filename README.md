# English-to-Hinglish Translation

This Python script provides a simple English to Hinglish translation tool using the MarianMT model from Hugging Face Transformers. It allows users to translate English sentences into Hinglish, a blend of Hindi and English, commonly used in informal communication.

## Approach

The English-to-Hinglish translation script uses the Hugging Face Transformers library to leverage the pre-trained MarianMT model for English-to-Hindi translation. The translation process follows these steps:

1. Load the pre-trained MarianMT model and tokenizer for English to Hindi translation.
2. Tokenize the input English sentence into words and perform part-of-speech tagging to identify nouns and verbs.
3. Create a dictionary of custom translations for specific English words that should remain in English during translation.
4. Translate the identified nouns and verbs to Hinglish using the model.
5. Translate the entire English sentence to Hinglish using the model.
6. Replace the translated nouns and verbs back to their English counterparts in the Hinglish sentence.
7. Handle plural forms or other specific replacements as needed.

The script provides translations that sound natural and are easy to understand for non-native Hindi speakers while keeping certain English words intact for ease of comprehension.

## Usage

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/english-to-hinglish-translation.git
   ```

2. Navigate to the project directory:

   ```bash
   cd english-to-hinglish-translation
   ```

3. Install the required Python packages:

   ```bash
   pip install transformers
   pip install nltk
   pip install sentencepiece
   ```

### Running the Script

To translate an English sentence to Hinglish, run the script with the following command:

```bash
python translate_to_hinglish.py "Your English sentence here."
```

The script will output the translated Hinglish sentence.

### Sample Output

English: 1. Definitely share your feedback in the comment section.
Hinglish: 1 निश्चित रूप से comment खण्ड में आपकी feedback share करें.

English: 2. So even if it's a big video, I will clearly mention all the products.
Hinglish: 2 अगर यह एक बड़ा video है, तो भी मैं स्पष्ट रूप से सभी products का mention करेंगे।

English: 3. I was waiting for my bag.
Hinglish: 3 मैं अपने बैग के लिए wait कर रहा था.

## Evaluation

The translation accuracy of the script depends on the quality of the pre-trained model and the complexity of the input sentences. For simple and common sentences, the translation should be accurate. However, for highly specialized or technical content, the accuracy may vary.

To evaluate the performance of the script, you can use reference translations for a set of English sentences and compare the script's translations against them. You can calculate metrics such as BLEU score, METEOR, or TER to assess the quality of translations quantitatively.

To evaluate the script on your own dataset, follow these steps:

1. Prepare a dataset of English sentences with reference Hinglish translations.
2. Modify the script to read sentences from your dataset for evaluation.
3. Use evaluation metrics or human evaluation to assess the script's translation quality.

Please note that this script is designed for informal communication and may not be suitable for professional or critical translation tasks.

## Contributing

Contributions to this project are welcome! If you have ideas for improvements, bug fixes, or new features, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
