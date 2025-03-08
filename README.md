# How Effectively Can BERT Models Interpret Context and Detect Bengali Communal Violent Text?

This repository provides the official implementation of the paper [How Effectively Can BERT Models Interpret Context and Detect Bengali Communal Violent Text?](https://drive.google.com/file/d/15_jEb3M5U4233wFxr_bBEXXClxXc4M5R/view?usp=sharing).

## 📝 Abstract
The spread of cyber hatred has led to communal violence, fueling aggression and conflicts between various religious, ethnic, and social groups, posing a significant threat to social harmony. Despite its critical importance, the classification of communal violent text remains an underexplored area in existing research. This study aims to enhance the accuracy of detecting text that incites communal violence, focusing specifically on Bengali textual data sourced from social media platforms. 

We introduce a fine-tuned **BanglaBERT** model tailored for this task, achieving a **macro F1 score of 0.60**. To address the issue of data imbalance, our dataset was expanded by adding **1,794 instances**, which facilitated the development and evaluation of a fine-tuned **ensemble model**. This ensemble model demonstrated improved performance, achieving a **macro F1 score of 0.63**, thus highlighting its effectiveness in this domain. 

In addition to quantitative performance metrics, qualitative analysis revealed instances where the models struggled with context understanding, leading to occasional misclassifications, even when predictions were made with high confidence. Through analyzing the cosine similarity between words, we identified certain limitations in the pre-trained BanglaBERT models, particularly in their ability to distinguish between closely related communal and non-communal terms. To further interpret the model’s decisions, we applied **LIME (Local Interpretable Model-Agnostic Explanations)**, which helped to uncover specific areas where the model struggled in understanding context, contributing to errors in classification. These findings highlight the promise of NLP and interpretability tools in reducing online communal violence. Our work contributes to the growing body of research in communal violence detection and offers a foundation for future studies aiming to refine these techniques for better accuracy and societal impact.

---

## 📂 Dataset
The dataset used in this research can be downloaded from the following link:  
🔗 [Download Dataset](https://drive.google.com/file/d/1HjA0O_-bfb-SxYvZhw8oPget5KpwISfl/view?usp=sharing)

---

## 🚀 Training
The training process was conducted in **Google Colab**.  
To replicate the training, place the dataset in the appropriate folders and execute the training notebook.

---

## 📊 Evaluation
To evaluate the trained model, follow the same folder structure used in the Colab training file and run the evaluation script.

---

## 🔥 Results
Our model achieved the following performance:

| Model Name                | Macro F1 Score |
|---------------------------|---------------|
| Fine-tuned **BanglaBERT** | **0.60** |
| Fine-tuned **Ensemble Model** | **0.63** |

---

## 📜 Citation
If you use this work in your research, please cite it as:

```bibtex
@misc{khondoker2024bert,
    title={How Effectively Can BERT Models Interpret Context and Detect Bengali Communal Violent Text?},
    author={Abdullah Khondoker and Enam Ahmed Taufik and Md Iftekhar Islam Tashik and S M Ishtiak Mahmud},
    year={2024},
    eprint={2412.18440},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
