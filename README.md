# LM-DB: a database powered by language models
### "LMs are all you need"
This project introduces a new type of database that uses Language Models (LMs) to perform all operations. The main objective is to allow users to interact with the database using natural language, which is then interpreted by an LM and executed on a text-based data store.

The data store used in this project is a flat file where each line represents a separate entry in the database. This was chosen for simplicity and because it is well-suited for the iterative approach we use for queries.

For inserting data and querying, we use natural language inputs which are then processed by the LM. The LM interprets the input and generates appropriate commands for the database operations.

For queries, each entry in the database is looped through and the LM is used to check if it meets the given criteria.

## How it Works
Data Insertion: Users input natural language commands for data insertion. The LM processes these commands and translates them into the appropriate format for the database. The data is then inserted into the text file.

Data Query: Users input natural language queries. The LM processes these queries and generates criteria for filtering the database entries. The system then loops through each entry in the database and uses the LM to check if the entry meets the criteria.

## Project Structure
This project consists of the following main components:

1. LM API: This is the interface for interaction with the Large Language Model. It includes methods for processing natural language commands and queries.

2. Database Manager: This module manages the database file, including insertion and retrieval of data.

3. Command Processor: This module processes the LM's responses and executes the corresponding database operations.

4. Tests: Unit tests for ensuring the correct functionality of the above components.
