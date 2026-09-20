Dictionary and Vocabulary Builder

A desktop application designed to help users look up English words, learn their definitions and pronunciations, and build a personalized vocabulary list. The application integrates a live REST API for dictionary data and a local SQLite database for saving words, featuring a responsive, multi-tabbed JavaFX interface.

Core Features

    Live Word Search: A dedicated search interface that queries a free dictionary JSON API to retrieve real-time English word data.

    Asynchronous Data Fetching: Network requests and JSON parsing are executed on a background thread, ensuring the main JavaFX GUI remains perfectly responsive while waiting for the API.

    Comprehensive Word Details: Parses the API response to display the searched word's definitions, parts of speech, and phonetic spellings.

    Personal Vocabulary Database: A save function that writes selected words directly to a local SQLite database for long-term study and memorization.

    Saved Words Dashboard: A separate GUI tab that queries the SQLite database to display an interactive list of all saved vocabulary words, allowing users to review and manage their collection.

Technical Stack:

    Language: Java

    Framework: JavaFX (UI and Tabbed Navigation)

    Database: SQLite with JDBC

    Concurrency: Java Multithreading / Task API (Background API requests)

    Data Parsing: JSON processing (e.g., using org.json or Gson)