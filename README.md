# Amazon Prime Video India: Customer Sentiment Analysis and Rating Drivers
## Project Overview
This project uses advanced Machine Learning (ML) and natural language processing (NLP) techniques to analyze over 2.5 lakh (250,000+) customer reviews of the Amazon Prime Video application from the Google Play Store in India.

The primary goal is to identify and quantify the specific factors (both positive and negative) that are driving the app's relatively low average rating (approximately 3.7) compared to major OTT competitors like Netflix and Hotstar.

## Data:
The primary dataset containing over 2.5 lakh customer reviews, ratings, and timestamps.


## Methodology
The analysis follows a two-stage approach:

Topic Modeling (LDA): Latent Dirichlet Allocation (LDA) is used to uncover the 8 most prevalent, latent discussion themes (topics) within the massive volume of customer reviews.

Regression Analysis: The proportion of each identified topic in a review is used as a feature to predict the user's given star rating (Ratings column). This quantifies the exact impact (positive or negative) each theme has on the final score.

## Key Findings (Project Conclusions)

Quantifiable Impact: Regression analysis (XGBoost) successfully predicted user ratings with an R-square score of approximately 0.63, statistically linking topic presence to rating outcomes.

Dominant Positive Driver: The single most important factor for high ratings is the Content Library (Positive Feedback & Content Library).

Top Pain Points: The largest negative drivers influencing the low 3.7 average rating were Advertising & Commercials and Technical Performance & Bugs.

Actionable Insights: Fixing technical stability and re-evaluating the ad placement strategy will yield the greatest immediate improvement in customer satisfaction.



## Key Segments

-- Segment 1: Data Loading and Preprocessing

-- Segment 2: LDA Model Training and Coherence Calculation

-- Segment 3: Regression Analysis (OLS, XGBoost, Stacking)

-- Segment 4: SHAP Visualization (Feature Importance)


## Topic Interpretation


#### Topic 0  :"watch", "show", "find", "back", "season", "make", "want", "go", "start", "use"

-Content Discovery and Navigation

#### Topic 1 : "movie", "love", "show", "use", "easy", "enjoy", "selection", "lot", "nice", "thank"

-Positive Experience & Content Library

#### Topic 2 : "pay", "movie", "free", "money", "membership", "charge", "rent", "new", "extra", "even

-Pricing and Subscription Issues

#### Topic 3 :"download", "account", "try", "even", "say", "use", "sign", "bad", "log", "login"

-Account & Login Problems

#### Topic 4 : "ad", "pay", "commercial", "add", "minute", "many", "get", "watch", "even", "still"

-Advertising/Commercial Interruptions

#### Topic 5 : "rent", "buy", "movie", "bad", "purchase", "take", "well", "see", "want", "ever"

-Rental and Purchase Experience

#### Topic 6 : "option", "need", "feature", "language", "add", "speed", "subtitle", "search", "brightness", "player"

-Features and Functionality

#### Topic 7 : "work", "phone", "update", "issue", "fix", "audio", "play", "open", "even", "crash"

-Technical Performance & Bugs
