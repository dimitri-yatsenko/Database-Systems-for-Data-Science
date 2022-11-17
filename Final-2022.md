# Database design project:  Online Quiz System

Design the database to support an online quiz system that stores multiple-choice questions and answers on different topics. 
Your submission should be a single jupyter notebook with separate sections for Schema Design, Populate, and Queries.
All code should be written in Python -- no SQL Magic. 
Name your schema `<username>_final`.


## Schema Design

The database design must support and enforce the following business rules.

1. The system will offer quizes on three subjects: *Database Systems*, *Machine Learning*, and *Scientific Visualization*.

2. The system will store mulitiple-choice questions for each subject. 

3. Each question is text, up to 2000 characters.

4. Each quesiton has three alternative textual answers up to 300 characters in lenth. Exactly one of the three questions is the correct answer.

5. The system allows quiz takers to register and to take quizes. 

6. Any quiz taker is allowed to take a quiz only once in each calendar year on any subject.

7. Each quiz randomly select 25 questions on one subject and presents them to the user. Each quiz only covers one subject.

8. The user supplies her answers to a subset of the quiz questions. The system records the responses.

9. The table records quiz scores expressed as the number of correct answers. 

Review the queries below to make sure that your database stores all the required informaiton.


## Populate 

1. Populate the database with 100 questions for each of the subjects and their corresponding answers. You can use the `faker` module to make up the text of both the questions and the answers.

2. Populate the database with 5000 quiz takers, identified by their `user_id`.

3. Write the function `make_quiz(user_id, subject, date)` which generates and records a quiz comprising 25 questions on the subject, each with three  answer choices.

4. Write the function `submit_quiz(user_id, subject, date, responses)`, which records the quiz taker's responses.

5. Invoke the funciton `make_quiz` and `submit_quiz` at least 10,000 times for random users, dates, and subjects. The date range should includ 2020-2022 inclusively. If your calls result in rejected duplicate entries, you will end up with fewer than 10,000 recorded quizes --- that's okay. 


## Queries

Write the following queries to your database. The calls must be made from Python.

1. Show the quiz takers' names of the 10 most recent quizes in  *Database Systems*, including their scores.

2. Show the top 10 best scores on *Scientific Visualization* in 2022, including the user names. 

3. Show the top 10 users who have taken most quizes across all years and subjects.

4. Show the 10 youngest users who have scored 85% or better in *Machine Learning* but have not taken a quiz in Database Systems.

5. Show the top 10 most difficult questions in *Machine Learning*, i.e. those questions that have been aswered wrong the most times.

6. Show all users who have scored 85% or better on all three subjects.

7. Show the number of quizes taken for each of the three subjects.

8. Show the number of unique quize takers for each of the three subjects.


