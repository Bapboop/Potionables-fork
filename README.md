Potionable is a fantasy theme take on Instructables where users are able to create fantasy inspired "recipes" as wel as share their own creations.
Live link: https://potionable.herokuapp.com/

![image](https://user-images.githubusercontent.com/6257940/160671159-2bf70192-4cbe-4ccd-a3ce-020098220301.png)


Users can view and leave comments on recipes.
![image](https://user-images.githubusercontent.com/6257940/160677606-7e5141ea-b4f9-4fe4-87fa-61d5dae7da95.png)

Users can also create their own recipes:
![image](https://user-images.githubusercontent.com/6257940/160678103-ab7a9a8a-8292-4874-b9cf-010e498aca50.png)


Technologies Used
Backend:

Python
Flask
Flask WTF & WTForms
SQLAlchemy
PostgreSQL
Docker
Heroku

Frontend:

JavaScript
React
Redux
Styled Components



Development:
To get started with contributing to the repo, follow the steps below:

Clone the repository
Install dependencies
pipenv install --dev -r dev-requirements.txt && pipenv install -r requirements.txt
cd react-app && npm install
Create a .env file based on the .env.example with the proper settings for your development environment
Set up your PostgreSQL user and database and make sure it matches the information in the .env
Get into pipenv and get the database up to date:
pipenv shell
flask db upprade
flask seed all
Start development servers
flask run
npm start
Installing new dependencies
If you add any python dependencies to your pipfiles (using pipenv install), you'll need to regenerate the requirements.txt before deployment.

For production dependencies, run pipenv lock -r > requirements.txt.

For development dependencies, run pipenv lock -r --dev > dev-requirements.txt.

Note: psycopg2-binary MUST remain a dev dependency because you can't install it on apline-linux. There is a layer in the Dockerfile that will install psycopg2 (not binary) for us.
# Potionables-fork
