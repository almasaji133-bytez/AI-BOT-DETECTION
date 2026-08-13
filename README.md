# AI-Based Detection of Social Media Bot Accounts Using Behavioral and Textual Analysis

## 📌 Project Overview

Social media platforms contain both genuine users and automated accounts (bots).
Bot accounts can be used to spread spam, manipulate discussions, and artificially
increase the visibility of certain content.

This project aims to detect Twitter/X bot accounts using **Machine Learning**
by combining two different types of information:

1. **Behavioral features** — information about how an account behaves.
2. **Textual features** — patterns found in the tweets posted by an account.

The project uses the **Cresci-2017 dataset**, which contains genuine Twitter
accounts and different types of bot accounts.

---

## 🎯 Objectives

- Explore and clean the Cresci-2017 dataset.
- Extract meaningful behavioral features from user accounts.
- Extract textual features from tweets.
- Train a machine learning model using behavioral features.
- Train a separate machine learning model using textual features.
- Combine the behavioral and textual information to improve bot detection.
- Evaluate the performance of the final model.

---

## 🧠 Proposed Approach

The overall pipeline of the project is:

Raw Dataset
↓
Data Cleaning
↓
Feature Extraction
↓
┌─────────────────────┬─────────────────────┐
│ Behavioral Features │ Textual Features │
└──────────┬──────────┴──────────┬──────────┘
↓ ↓
Behavior Model Text Model
│ │
└──────────┬──────────┘
↓
Feature / Model Fusion
↓
Final Prediction
↓
Bot or Genuine User

---

## 📊 Dataset

### Cresci-2017

The Cresci-2017 dataset contains Twitter accounts belonging to different
categories, including:

- Genuine accounts
- Traditional spambots
- Social spambots

The dataset contains user-level information in `users.csv` and tweet-level
information in `tweets.csv`.

The raw dataset is **not stored in this repository** because of its large size.

### Dataset Setup

After downloading the dataset, place it inside:

```text
data/raw/
```
