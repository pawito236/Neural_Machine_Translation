# Neural Machine Translation
 Cleansing corpus, Using USE to select best translation and Finetune pretrained model([Helsinki-NLP/opus-mt-th-en](https://huggingface.co/Helsinki-NLP/opus-mt-th-en))
## Multilingual Universal Sentence Encoder
![USE-2](https://user-images.githubusercontent.com/44425803/163429640-e90015e6-da37-47bf-b1ad-329569695ab3.png)
1. นำข้อมูลทั้งไทย และ อังกฤษมา ทำ Sentence Embedding ด้วย (USE)
2. หา Distance ในที่นี้ผมใช้ Cosine Similarity
3. หา Threshold ในการตัดว่า range ไหนถึงเป็นคู่ประโยคที่ถูกต้อง

## References and Related repos
[ตรวจสอบความถูกต้องของการแปล ด้วย Universal Sentence Encoder](https://medium.com/airesearch-in-th/%E0%B8%95%E0%B8%A3%E0%B8%A7%E0%B8%88%E0%B8%AA%E0%B8%AD%E0%B8%9A%E0%B8%84%E0%B8%A7%E0%B8%B2%E0%B8%A1%E0%B8%96%E0%B8%B9%E0%B8%81%E0%B8%95%E0%B9%89%E0%B8%AD%E0%B8%87%E0%B8%82%E0%B8%AD%E0%B8%87%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%81%E0%B8%9B%E0%B8%A5-%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2-universal-sentence-encoder-ad3c156c2e9b)

[Helsinki-NLP/opus-mt-th-en](https://huggingface.co/Helsinki-NLP/opus-mt-th-en) Pre-trained model

## Medium
[Neural Machine Translation](https://medium.com/@pawito236/neural-machine-translation-675360e2df34) Explore overview of NMT also the pros and cons of each model. Focus on Transformer model what is the advantage from RNN or LSTM and its architecture.
Clean corpus and use Transformer model with pre-trained from Huggingface(Helsinki-NLP/opus-mt-th-en). Then use Multilingual Universal Sentence Encoder (USE) to select Best translation from cousine-similarity score.

## Future Work
Try [SentencePiece independent subword tokenizer and detokenizer for Neural Text Processing](https://medium.com/@pawito236/sentencepiece-a-simple-and-language-independent-subword-tokenizer-and-detokenizer-for-neural-text-2c57ea3abc1c)
