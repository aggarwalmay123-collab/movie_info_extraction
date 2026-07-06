# 🎬 Movie Information Extraction Tool (CineSage)

The **Movie Information Extraction Tool** is an AI-powered component of the **CineSage** project that extracts structured information from natural language movie-related queries. Instead of requiring users to search through large datasets manually, the tool understands user requests and returns organized movie details in a structured format.

## Features

* 🎥 Extracts movie titles from user queries.
* 🌍 Identifies the language of the movie (if mentioned).
* 🎭 Detects one or more genres.
* ⭐ Extracts IMDb rating constraints.
* 📅 Recognizes release year or year range.
* 👥 Identifies cast members and directors.
* 📝 Detects keywords, themes, or plot-related information.
* 📊 Returns structured JSON output for downstream applications.
* 🤖 Powered by Large Language Models (LLMs) for accurate natural language understanding.

## Tech Stack

* Python
* Streamlit
* LangChain
* Mistral AI
* Pydantic
* Prompt Engineering

## How It Works

1. The user enters a movie-related query in natural language.
2. The query is sent to the LLM using a carefully designed prompt.
3. The LLM extracts relevant movie attributes.
4. Pydantic validates the extracted information.
5. The application displays the structured output in an easy-to-read format.

## Example

**Input Query**

> "Recommend action movies released after 2018 with an IMDb rating above 8 starring Keanu Reeves."

**Extracted Output**

```json
{
  "title": null,
  "genres": ["Action"],
  "release_year": ">2018",
  "imdb_rating": ">8.0",
  "cast": ["Keanu Reeves"],
  "director": null,
  "language": null,
  "keywords": ["recommend"]
}
```

## Applications

* AI Movie Recommendation Systems
* Semantic Movie Search
* Conversational Movie Assistants
* Entertainment Chatbots
* Movie Database Query Automation

## Future Improvements

* Integration with TMDb and OMDb APIs for real-time movie information.
* Support for multilingual queries.
* Personalized recommendations based on user preferences.
* Voice-based movie search.
* Advanced filtering using runtime, country, streaming platform, and awards.
