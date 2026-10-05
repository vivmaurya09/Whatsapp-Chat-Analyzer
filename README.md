#WhatsApp Chat Analyzer
### Prerequisites

Make sure you have the following installed:

- Python 3.8 or higher
- Streamlit
- Required Python packages: `pandas`, `seaborn`, `matplotlib`, `plotly`, `wordcloud`, `emoji`, `urlextract`, `nltk`

## Table of Contents

- [Introduction](#introduction)
- [Demo](#demo)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)

## Introduction

The **WhatsApp Chat Analyzer** is designed to help you gain valuable insights from your WhatsApp chats. It provides various functionalities to analyze and visualize data extracted from the chat exports. This tool allows you to explore patterns, trends, and statistics related to your conversations, helping you understand your messaging behavior and communication patterns.

## Demo

Check out the live demo of the WhatsAppChatAnalzyer App:  [https://pm2c0h55-8501.inc1.devtunnels.ms/]

> *If the website does not load properly, try opening it in incognito mode.*

## 🎯 Features

- **Top Statistics**: Get an overview of the total messages, words, media shared, and links shared in the chat.
- **Monthly Timeline**: Visualize the number of messages exchanged each month.
- **Daily Timeline**: Track daily messaging activity.
- **Activity Map**: Discover the most active days and months in your chat.
- **Weekly Activity Map**: Heatmap showing the messaging activity throughout the week.
- **Most Active Users**: Identify the most active participants in the chat.
- **Wordcloud**: Generate a wordcloud of the most frequently used words in the chat.
- **Most Common Words**: List the most common words used in the chat.
- **Supports 12-Hour Time Format**: Specifically designed to work with WhatsApp chats exported in 12-hour time format.

## Installation

To get a local copy of this project up and running, follow these steps:

1. Clone this repository to your local machine using the following command:

   ```shell
   git clone https://github.com/vivmaurya09/Whatsapp-Chat-Analyzer.git
2. Navigate to the project directory:
   ``` shell
   cd WhatsAppChatAnalzyer
   ```
3. Install the required dependencies:
   ``` shell
   pip install -r requirements.txt
   ```
4. Running the App:
   ``` shell
   streamlit run main.py
   ```
   This will start the app in the local environment

   ## Usage
- Export your WhatsApp chat conversation as a text file. You can find instructions on how to export chat logs on the WhatsApp website.
- Visit the  app [website](https://pm2c0h55-8501.inc1.devtunnels.ms/) or run the app in local environment.
- Upload the chat text file on the server.
- Follow the on-screen instructions to choose the desired analysis options.

## Examples
Here are a few examples of how you can use the WhatsApp Chat Analyzer tool:
- Analyze chat statistics for a group chat over a specific time period.
- Generate a word cloud to visualize the most frequently used words in a one-on-one conversation.
- View active participation in a group chat among multiple participants.

> The WhatsAppChatAnalzyer App was developed just for learning purposes.
> 
> Feel free to customize and enhance the App according to your needs. Happy WhatsApp chat analysis!

## 🧠 How It Works

1. **Data Preprocessing:**
   - The uploaded chat file is converted from bytes to a string.
   - Dates, times, and messages are extracted using regular expressions.
   - The chat data is then processed to separate user names and messages, which are stored in a pandas DataFrame.

2. **Analysis:**
   - **Top Statistics:** Computes the total number of messages, words, media files, and links shared.
   - **Timelines:** Visualize messaging activity over time using monthly and daily timelines.
   - **Activity Maps:** Understand the most active days of the week and months of the year.
   - **Wordcloud & Common Words:** Generate a wordcloud and identify the most common words used in the chat.
   - **Heatmap:** Displays weekly activity based on the time of day and day of the week.
   - **Most Active Users:** For group chats, identify the most active participants.

3. **Visualization:**
   - Interactive plots and charts are generated using `matplotlib`, `seaborn`, and `plotly`.
   - A wordcloud is created using the `WordCloud` library to highlight frequently used words.
