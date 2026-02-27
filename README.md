# Data Analysis Challenge - Team 9

This project analyzes a social media dataset to answer six questions assigned.

This repository contains all code, documentation, and visual outputs required for the assignment.

---
## Repository Structure:
**Data**: team09_social_media.csv
**Notebook**: DataChallenge2P08.ipynb
**Visuals**: TBD
README.md

---
## Environmnt and Tools Used
- Python 3
- Pandas
- Numpy
- Google Collab

---
## Project Workflow

### Step 1: Data Exploration
- Loaded Dataset into Pandas
- Reviewed structure and data types
- Identified missing values
- Checked for invalid or inconsistent entries
- Examined summary stats

### Step 2: Data Cleaning
- Handled mising values
  - 74 missing *likes*, 50 missing *follower_count*
  - We chose to fill them in with the median since social media engagement often contains outliers that we skew the mean.
- Converted incorrect data types
  - All that we had to correct was the time/date format on post date.

---
### Step 3: Analysis
**1. Which post type receives the most engagement (likes + comments + shares)?**
    - Photo posts recieed the most engagement on average with an average of 124.13, the next runner up being the "link" at 121.37.
**2. What time of day generates the highest average likes?**
    - Afternoon posts recieved the highest average likes with a average like count of 109.35, while the runner up having an average of 100.73 Morning
**3. How does follower count correlate with engagement?**
        - There is almost no correlation between follower count and engagement since the correlation value is 0.0139.
**4. What is the optimal number of hashtags for maximum engagement?**
    - 9 at first shows up as the best engagement, but due to it being an outlier with only 1 post we cannot accept that as an answer. When we limit our consideration to atleast 5 posts, there is a answer of '0' with 128.82 or '6' with 128.58.
**5. Which post type has the highest share rate?**
    - Videos posts are the most shared with an average share of 4.7, next runner up being the text with 4.61.
**6. How does engagement vary by month?**
    - July has the highest average engagement with an average of 142.10, the runner up being April with an average of 127.72

**Answering Structure**:
- The question statement
- Code implementation
- Results
