# Optical Music Recognition Using Vision Transformers

General Architecture:

This model makes use of (by modifying and adapting) the encoder-decoder transformer architecture, proposed by Li et al. (2023), called TrOCR. TrOCR is a model trained for the purpose of OCR, primarily for the English language (alphabet). To be more specific, we will be using the TrOCR-SMALL variant, designed to be more data efficient (total parameters = 62 million). Instead of using this architecture and training from scratch, we utilize the pre-trained weights from TrOCR to see take advantage of transfer learning (even though this model is trained primarily for English based OCR and has no OMR related training). The model also uses a different tokenizer than what the model comes with.

Following is a diagram of the general architecture:

![alt text](image.png)

