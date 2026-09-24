# What Makes a Good Book? (Python)

**Background:** Identifying popular products is incredibly important for e-commerce companies! Popular products generate more revenue and, therefore, play a key role in stock control.

**Purpose:** You've been asked to support an online bookstore by building a model to predict whether a book will be popular or not. They have high expectations & have set a target of at least 70% accuracy. You are free to use as many features as you like, and will need to engineer new features to achieve this level of performance.

**File Note:** The dataset file exceeded the file size allowed by Github (~28 MB), so it could not be uploaded to this repository.

This project was done in January, 2026. Machine learning was utilized.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Objectives
Build a model that predicts whether a book will be rated as popular or not.  The model must have an accuracy of at least 70%.


### Brief Summary
The dataset utilized revolved around books that have been sold & their characteristics like title, author, category, price, & a label deeming them popular or unpopular. Details concerning readers' reviews were also included.  
A brief evaluation of the dataset revealed that there was only one missing value among 15,719. Of these reviews, 10,490 labeled a book "Unpopular" & 5,229 labeled a book "Popular"; about a 2:1 ratio.

Multiple preprocessing steps were utilized to prepare the dataset including the creation of new variables, data standardization, & transformations. A random forest classifier, along with a random search cross-validation, were built & executed.  
The feature variables used included the book price, the number of helpful & total reviews, the percentage of helpful reviews, the book category, as well as the number of positive words in each book's description & in each reader's full review & review summary. These "positive" words were chosen specifically according to how likely they are to be associated with reviews of popular books.

> Ultimately, the model produced yielded an accuracy score of about 70.3%.

Following the modeling process, the feature variables were analyzed to determine which were the most important in terms of predicting whether books were deemed popular or not. Of them, the book **price** was by far the most important. Five other variables also had a relatively notable importance:
- The number of positive words in a reader's full review.
- The number of total reviews published of a book.
- The percentage of reviews deemed helpful of a book.
- The number of positive words in a book's description.
- The number of helpful reviews published of a book.

A more in-depth summary can be found in the project.


### Recommendations
To achieve a model that achieves the desired predictive capabilities, a random forest classifier can be used with the particular hyperparameter values & feature variables found in the project.

Of course, the model could possibly be optimized beyond what was done in this instance. Further experimentation could explore alternative machine learning algorithms, different interpretations & implementations of the text variables, & different sets of feature variables to try & elevate the model's predictive capabilities.  
On another note, by continuing to obtain & sell books, thus compiling more data, it can help contribute towards building more powerful predictive models that are more flexible & accurate in evaluating whether books will be labeled as popular or not.

Ultimately, a bookstore will naturally be interested in obtaining popular books because they are easier to sell to customers. By utilizing modeling processes defined in this project, the bookstore can more easily find characteristics & trends of books that are more likely to be associated with "popular" books. By obtaining such books, the bookstore can potentially become more efficient in their sales because customers are naturally more interested in more appealing products. The more sales the bookstore experiences, the more they will drive up important business metrics like purchases & revenue, popularity, competitiveness/relevance/recognition, flexibility, & additional measures of success.

Furthermore, for a business like a book store, identifying popular products will be very beneficial when it comes to stock management & areas such as inventory tracking & demand forecasting. For example, identifying the most popular book categories will help the bookstore gauge how often they need to resupply their inventories across these categories in addition to projecting how many books might be sold, thus giving them an impression & reasonable goals as to potential ranges of sales in the future (e.g. monthly, quarterly, annually).

Such characteristics in particular, based on books that have been sold by the bookstore, can be referenced in the project; specifically in the **Analysis II - Feature Variable Analysis** section.
