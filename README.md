# Book Recommendation System using K-Nearest Neighbors (KNN)

## Overview
This project implements a book recommendation system using the K-Nearest Neighbors (KNN) algorithm. It is built using Python and utilizes the Book-Crossing dataset, which contains over 1.1 million ratings of 270,000 books by 90,000 users.

## Dataset
The Book-Crossing dataset consists of three CSV files:
- **Books.csv**: Contains information about books (ISBN, title, author, etc.)
- **Ratings.csv**: Contains book ratings given by users
- **Users.csv**: Contains user demographic information

## Project Features
- Cleans and preprocesses the dataset
- Filters out users with fewer than 200 ratings and books with fewer than 100 ratings to ensure statistical significance
- Creates a user-book pivot table
- Implements a KNN model to recommend similar books based on user preferences
- Provides a function `get_recommends(book_title)` to return the top 5 recommended books for a given book title

## Installation & Usage
### Prerequisites
Ensure you have Python installed along with the following libraries:
```bash
pip install pandas scikit-learn scipy
```

### Running the Project
1. Clone this repository:
```bash
git clone https://github.com/your-username/book-recommendation-knn.git
```
2. Navigate to the project folder and run the Jupyter Notebook or Python script.
3. Load the datasets and execute the script.
4. Use the function to get book recommendations:
```python
get_recommends("Catch-22")
```

## Example Output
```python
get_recommends("Catch-22")
```
Returns:
```python
['Catch-22',
 [['Book1', 0.793],
  ['Book2', 0.744],
  ['Book3', 0.734],
  ['Book4', 0.537],
  ['Book5', 0.517]]]
```

## Project Structure
```
|-- Book Recommendation Knn.ipynb
|-- Books.csv
|-- Ratings.csv
|-- Users.csv
|-- README.md
```

## License
This project is for educational purposes. You may modify and distribute it as needed.

## Author
[Ranjeeth Kumar Patra](https://github.com/your-username)

