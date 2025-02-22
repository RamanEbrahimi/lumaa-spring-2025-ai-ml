# AI/Machine Learning Intern Challenge: Simple Content-Based Recommendation

**Deadline**: Sunday, Feb 23th 11:59 pm PST

---

## Overview

Build a **content-based recommendation system** that, given a **short text description** of a user’s preferences, suggests **similar items** (e.g., movies) from a small dataset. This challenge should take about **3 hours**, so keep your solution **simple** yet **functional**.

### Example Use Case

- The user inputs:  
  *"I love thrilling action movies set in space, with a comedic twist."*  
- Your system processes this description (query) and compares it to a dataset of items (e.g., movies with their plot summaries or keywords).  
- You then return the **top 3–5 “closest” matches** to the user.

---

# Dataset

This system uses two CSV files:

**movies.csv**: Contains movie details including movieId, title, and genres.

**ratings.csv**: Contains user ratings with columns userId, movieId, rating, and timestamp.

Ensure these files are in the Data directory. If you relocate them then you must change the lines:
```
movie_file = 'Data/movies.csv'

rating_file = 'Data/ratings.csv'
```

---

# Setup

Prerequisites

Python version: 3.8+

Install dependencies using:
```
pip install -r requirements.txt
```

---

# Running the Code

Run the Jupyter Notebook and execute the script interactively.

When prompted:

Enter ```1``` for content-based recommendation or ```2``` for hybrid recommendation.

For content-based filtering, enter a movie description (e.g., *"I like action movies set in space"*).

For hybrid filtering, enter your ```userId```.

---

# Example Output

```
Enter '1' for content-based or '2' for hybrid recommendation: 1
Enter movie description preferences: Action adventure fantasy
Recommended Movies:
Mad Max: Fury Road (Score: 0.82)
Guardians of the Galaxy (Score: 0.79)
Interstellar (Score: 0.75)

Enter '1' for content-based or '2' for hybrid recommendation: 2
Enter your user ID: 3
Recommended Movies:
The Dark Knight (Score: 4.8)
Inception (Score: 4.7)
The Matrix (Score: 4.6)
```






