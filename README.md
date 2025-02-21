# MySQL-Project-on-Movie-Dataset

# Movie Database Datasets

This repository contains multiple datasets related to movies, actors, directors, genres, ratings, and reviews. These datasets are structured in CSV format and can be used for SQL queries, data analysis, and visualization.

## 📂 Dataset Descriptions

### 1️⃣ **actor.csv**
- **Description:** Contains details of actors, including their names and gender.
- **Columns:**
  - `act_id` → Unique ID of the actor
  - `act_fname` → First name of the actor
  - `act_lname` → Last name of the actor
  - `act_gender` → Gender of the actor (`M` or `F`)

### 2️⃣ **cast.csv**
- **Description:** Stores information about which actor played which role in which movie.
- **Columns:**
  - `act_id` → Actor's ID (Foreign Key from `actor.csv`)
  - `mov_id` → Movie ID (Foreign Key from `movie.csv`)
  - `role` → Role played by the actor in the movie

### 3️⃣ **director.csv**
- **Description:** Contains details of directors.
- **Columns:**
  - `dir_id` → Unique ID of the director
  - `dir_fname` → First name of the director
  - `dir_lname` → Last name of the director

### 4️⃣ **genres.csv**
- **Description:** Stores different movie genres.
- **Columns:**
  - `gen_id` → Unique Genre ID
  - `gen_title` → Name of the genre (e.g., Action, Drama, Comedy)

### 5️⃣ **movie.csv**
- **Description:** Stores information about movies.
- **Columns:**
  - `mov_id` → Unique Movie ID
  - `mov_title` → Title of the movie
  - `mov_year` → Year of release
  - `mov_time` → Duration of the movie (in minutes)
  - `mov_lang` → Language of the movie
  - `mov_dt_rel` → Release date
  - `mov_rel_country` → Country of release

### 6️⃣ **movie_direction.csv**
- **Description:** Maps movies to their respective directors.
- **Columns:**
  - `mov_id` → Movie ID (Foreign Key from `movie.csv`)
  - `dir_id` → Director ID (Foreign Key from `director.csv`)

### 7️⃣ **movie_genres.csv**
- **Description:** Maps movies to their respective genres.
- **Columns:**
  - `mov_id` → Movie ID (Foreign Key from `movie.csv`)
  - `gen_id` → Genre ID (Foreign Key from `genres.csv`)

### 8️⃣ **ratings.csv**
- **Description:** Stores ratings given to movies by reviewers.
- **Columns:**
  - `mov_id` → Movie ID (Foreign Key from `movie.csv`)
  - `rev_id` → Reviewer ID (Foreign Key from `reviewer.csv`)
  - `rev_stars` → Rating given by the reviewer (out of 10)
  - `num_o_ratings` → Number of ratings received

### 9️⃣ **reviewer.csv**
- **Description:** Contains information about reviewers.
- **Columns:**
  - `rev_id` → Unique ID of the reviewer
  - `rev_name` → Name of the reviewer

## 🛠 **How to Use These Datasets**
- Load these datasets into a **SQL database** using `LOAD DATA INFILE` or a database GUI.
- Perform SQL queries to extract meaningful insights.
- Join tables using `INNER JOIN` to analyze relationships between movies, actors, directors, genres, and ratings.

## 📌 **License**
This dataset is free to use for educational and research purposes.

---
