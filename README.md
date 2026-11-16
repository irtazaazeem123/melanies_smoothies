<h1 align="center">🥤 Melanie's Smoothies: Custom Order App</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
</p>

A **Streamlit** web app backed by **Snowflake** that lets customers build and order a custom smoothie, with live nutrition information for each fruit.

## ✨ Features

- 📝 Enter a name for the order and pick **up to 5 fruits** from a list loaded live from a Snowflake table (`fruit_options`)
- 🍓 Shows **nutrition facts** for each selected fruit, fetched in real time from the public **Fruityvice API**
- ✅ **Submit Order** writes the order (ingredients + name) into a Snowflake `orders` table through **Snowpark**

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| UI | Streamlit |
| Data | Snowflake (Snowpark Python) |
| External API | Fruityvice (via `requests`) |

## 🚀 Run Locally

~~~bash
pip install -r requirements.txt
# add your Snowflake connection details to .streamlit/secrets.toml under [connections.snowflake]
streamlit run streamlit_app.py
~~~

---

👤 **Muhammad Irtaza Azeem** · [LinkedIn](https://www.linkedin.com/in/muhammad-irtaza-azeem) · [GitHub](https://github.com/irtazaazeem123)
