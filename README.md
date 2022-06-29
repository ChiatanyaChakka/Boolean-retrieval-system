# Boolean Retrieval system

## Project description
Boolean Retrieval Model is the first and most used classic information retrieval model. We make a few assumptions in the Boolean model, such as:
- If the given index term is present in the document, the value is 1; otherwise,
it is 0.
- Queries in the Boolean model are AND, OR, NOT. They represent the
following combinations
    - “X AND Y” represents a list of documents containing both X and Y.
    - “X OR Y” represents a list of documents containing either X or Y,
    - “NOT X” represents a list of documents not containing X.

### Preprocessing steps:
1. Converting all the document corpse data into lowercase.
2. Removing stopwords to remove unnecessary computation while searching
3. Stemming each word i.e.., removing suffixes and prefixes and reducing the word to its  "stem".
4. Building a permuterm and inverted index for the system to process the queries

## Scope
This Boolean Retrieval model takes a query as an input from the user. It analyses the query and fetches us the inverted index array of the recognised word. The recognised words are spelling corrected and then stemmed before fetching us the inverted index. For wildcard search query, we get all the words from the permuterm index, and then we get the
inverted index arrays for all the terms and perform OR operation. After getting inverted index arrays of all the words, it performs the boolean operations on the arrays given in the query.


