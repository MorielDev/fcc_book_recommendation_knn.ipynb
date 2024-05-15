Book Recommendation Engine using KNN - From FreeCodeCamp

This project aimed to develop a book recommendation engine using the K-Nearest Neighbors (KNN) algorithm. Below is a breakdown of the process, challenges encountered, and their solutions:

Overview:
Objective: To create a recommendation system that suggests books similar to a given book.
Dataset: Book-Crossings dataset containing 1.1 million ratings of 270,000 books by 90,000 users.
Process:
Data Import and Cleaning:

Imported the necessary libraries.
Loaded the dataset.
Performed data cleaning, including removing users with fewer than 200 ratings and books with fewer than 100 ratings.
Model Development:

Used NearestNeighbors from sklearn.neighbors to develop the recommendation model.
Developed the get_recommends() function to return a list of 5 similar books with their distances from the input book.
Testing:

Created a test function (test_book_recommendation()) to validate the functionality of the recommendation system.
Ran tests using predefined test cases to ensure the accuracy of the recommendations.
Challenges Encountered:
Index Errors:

One common issue was IndexError, indicating that the index used to access elements in arrays or DataFrames was out of bounds.
Solution: This was typically due to incorrect indexing or mismatched array dimensions. Ensuring proper indexing and array reshaping resolved these errors.
Feature Names Warning:

A UserWarning was raised stating that the feature names were not valid, even though the NearestNeighbors model was fitted with feature names.
Solution: This warning could be ignored as it did not affect the functionality of the recommendation system.
Handling Missing Values:

The presence of missing values in the dataset could affect the accuracy of the recommendation model.
Solution: Missing values were handled by either removing the corresponding rows or filling them with mean ratings, depending on the context.
Debugging and Testing:

Debugging code to identify and fix errors, and ensuring the correctness of the recommendation system through comprehensive testing, was time-consuming.
Solution: Adopting a systematic approach to debugging, using print statements and visualization techniques, and conducting thorough testing with diverse test cases helped identify and resolve issues.
