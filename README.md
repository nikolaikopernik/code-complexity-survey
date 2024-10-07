# Code complexity survey
The idea of this project is to get an imperative code complexity based on user's feedback to 
code examples.

## Raw examples
There are some raw code examples generated from the popular open-source projects. Those 
examples can be found in data/exampels.db. It's a sqllite database with the following format:
```aiignore
create table main.examples
(
    id         TEXT primary key,
    lang       TEXT,
    complexity INTEGER,
    body       BLOB
);
```
There are currently 3 languages supported:
```aiignore
lang|examples
----|--------
java|154663
kotlin|24046
python|38317
```