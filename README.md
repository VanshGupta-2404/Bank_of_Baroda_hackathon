# 🧠 Personalized Banking Advertisement Generator and Email Sender

This project is a **machine learning and generative AI-powered solution** developed for the **Bank of Baroda Hackathon**. It automatically creates and delivers **personalized banking advertisements** based on customer profiles using a **Random Forest Classifier** and **DALL·E image generation** via **Azure OpenAI**.

---

## 📌 Table of Contents

* [🚀 Introduction](#-introduction)
* [🛠️ Requirements](#-requirements)
* [⚙️ Setup & Usage](#️-setup--usage)
* [🧪 Customization](#-customization)
* [🔐 Notes on Security](#-notes-on-security)
* [📫 Contact](#-contact)

---

## 🚀 Introduction

This project demonstrates the **intelligent automation of marketing** through:

* 📊 **Customer profiling via ML**
* 🎯 **Product targeting using a trained Random Forest model**
* 🎨 **Visual ad creation via DALL·E**
* ✉️ **Email delivery with personalization**

The system takes customer demographic and behavior data, predicts their most relevant banking product, generates an AI-created visual ad tailored to them, and delivers it via email.

---

## 🛠️ Requirements

Ensure the following packages are installed:

```bash
pip install pandas numpy scikit-learn joblib matplotlib pillow requests openai
```

---

## ⚙️ Setup & Usage

### 🔁 Step 1: Train the ML Model

```bash
python generate_and_train_model.py
```

* Trains a `RandomForestClassifier` on synthetic customer banking data.
* Saves the model as `model.pkl`.

### 🎨 Step 2: Generate and Send Personalized Ad

```bash
python generate_and_send_ad.py
```

* Predicts product category from customer profile.
* Generates a marketing image using Azure OpenAI's **DALL·E** API.
* Sends it as an email attachment to the customer.

---

## 🧪 Customization

| What You Can Change  | How                                                 |
| -------------------- | --------------------------------------------------- |
| 🧍 Customer Profile  | Update `example_data` in `generate_and_send_ad.py`. |
| ✉️ Email Content     | Edit `subject` and `body` fields.                   |
| 🔍 ML Model Settings | Modify `RandomForestClassifier` params.             |
| 🎨 Image Prompt      | Customize the prompt passed to OpenAI's API.        |

---

## 🔐 Notes on Security

* **Do NOT hardcode** email passwords in the script.
* Use **environment variables** or `.env` files for credentials.
* For Gmail, use **App Passwords** to avoid compromising your main account.
* **Model accuracy < 90%?** Consider:

  * Hyperparameter tuning
  * Feature engineering
  * Trying a different ML algorithm (e.g., XGBoost, SVM)

---

## 📫 Contact

For questions or collaboration opportunities:
📧 [guptavansh2404@gmail.com](mailto:guptavansh2404@gmail.com)


