# u-develop-it

![License](https://img.shields.io/badge/License-NONE-grenn.svg)
  
# Description

U Develop It is a voting back-end app for a developer gathering group.
The database is built with Sqlite3 ans have 4 tables.




# Table of Contents

[Installation](#Installation)

[Usage](#Usage)

[License](#License)

[Technologies](#Technologies)

[Questions](#Questions)

# Installation
 - Clone the app in to your pc.
- In the project directory run: `npm install` and then `sqlite3 --version`.
- In the project directory run: `sqlite3 db/election.db` and then `.schema`



# Usage
- The user can insert new candidates to the candidate table by running the query:
> - INSERT INTO candidates (industry_connected, last_name, first_name)
VALUES (1, 'Firbank', 'Ronald' );

- `Table of Candidates example.`

 ![candidates](/images/table-candidates.jpg)

  - The user can insert new voters to the voters table by running the query:

> - INSERT INTO voters (first_name, last_name, email)
VALUES
  ('James', 'Fraser', 'jf@goldenbough.edu'),
  ('Jack', 'London', 'jlondon@ualaska.edu'),
  ('Robert', 'Bruce', 'rbruce@scotland.net');

- `Table of Voters example.`

 ![voter](/images/table-voters.jpg)

   - The user can insert new parties to the parties table by running the query:

 INSERT INTO parties (name, description)
VALUES
  ('JS Juggernauts', 'The JS Juggernauts eat, breathe, and sleep JavaScript. They can build everything you could ever want in JS, including a new kitchen sink.'),
  ('Heroes of HTML', 'Want to see a mock-up turn into an actual webpage in a matter of minutes? Well, the Heroes of HTML can get it done in a matter of seconds.'),
  ('Git Gurus', 'Need to resolve a merge conflict? The Git Gurus have your back. Nobody knows Git like these folks do.');

- `Table of Parties example.`

 ![parties](/images/table-parties.jpg)


- The user can excute query like:
> -  SELECT * FROM candidates LEFT JOIN parties ON candidates.party_id = parties.id;
> - SELECT candidates.*, parties.name FROM candidates LEFT JOIN parties ON candidates.party_id = parties.id;
- All the queries CRUD (Create,REad,Update and Delete).




# License
The license for which the application is covered:NONE 


# Technologies 
- Node
- Express
- Inquirer
- Sqlite3
- Jest



# Questions

  If you have questions about the project, below you can find ways to answer them, either by visiting my github or contacting me by email
  
  Link to my Github: [anniavd](https://github.com/anniavd)

  
  Email acount: [annia.valdesd@gmail.com](mailto:annia.valdesd@gmail.com)
