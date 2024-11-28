
#### **Project Title**
Testing the McGurk Effect in Multimodal Machine Learning Models

---

#### **Abstract**
This project investigates the susceptibility of multimodal machine learning models to sensory conflicts using the McGurk Effect, an audio-visual illusion where mismatched cues create altered perception. By creating cohesive, mismatched, and adversarial datasets from the GRID audiovisual corpus, we evaluate three architectures—Bimodal Autoencoder, Multimodal Transformer, and Audio-Visual Convolutional Neural Network (AVCNN). The results reveal significant vulnerabilities in multimodal systems, emphasizing the need for more robust models in real-world applications.

---

#### **Objectives**
1. Simulate the McGurk Effect by creating mismatched audio-visual datasets.
2. Evaluate multimodal models' performance on congruent and incongruent input pairs.
3. Identify model architectures most resilient to sensory conflicts.
4. Provide insights into improving robustness in multimodal systems.

---

#### **Features**
- **Dataset Preprocessing:** 
  - **Audio:** Converted to Mel spectrograms (64 or 40 bands), normalized, and padded to consistent lengths.
  - **Video:** Extracted frames resized to 112x112 pixels, with an additional pipeline for mouth regions resized to 60x80 pixels.
  - **Alignment:** Paired audio and video features by phoneme timestamps.
- **Model Architectures Tested:**
  1. **Bimodal Autoencoder:** Encodes shared latent features of audio and video.
  2. **Multimodal Transformer:** Utilizes self-attention and cross-modal attention for phoneme classification.
  3. **AVCNN:** Tests robustness using adversarial perturbations.

---


---

#### **Results**
- **Bimodal Autoencoder:** Effectively captures shared features but struggles with mismatched pairs.
- **Transformer:** Achieved 88.78% training accuracy and 85.75% validation accuracy; simulates human-like predictions in 30% of cases.
- **AVCNN:** Demonstrated high susceptibility to adversarial mismatches, with 80% fooled predictions.

---

#### **Future Work**
- Extend analysis to include additional modalities.
- Test robustness across larger datasets and diverse real-world scenarios.
- Investigate whether increased data volume enhances or compromises model robustness.

---

#### **Contributors**
- **Satrajit Ghosh**  
  *ECE, Rutgers New Brunswick*  
  *Email:* sg2231@rutgers.edu  

---

#### **References**
1. [GRID Audiovisual Corpus](https://spandh.dcs.shef.ac.uk/gridcorpus/)
2. Related research papers cited in the methodology and results sections.

---

Feel free to customize this further or add links to specific sections of your repository!
