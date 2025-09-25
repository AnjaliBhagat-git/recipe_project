Software Engineer (Backend)– Coding Test
Assessment Criteria:
Objective
Acme Inc. is creating a recipe management application where users can create and manage ingredients and recipe. Create a backend application utilizing Django, Django Rest Framework and Graphene or Strawberry Django (for GraphQL).
Specification
We require GraphQL queries for the following:
1.
Create, Update, Delete ingredients in/from the database.
2.
List all ingredients from the database and also have filters and pagination while listing.
3.
Create a recipe and connect few ingredients to it (in the same request).
4.
Get details of a recipe and see all its ingredients
a. We want a calculated ingredient_count field for the recipe Node, which will give us the count of ingredients attached to a recipe. This should be a calculated field and not a database field.
5.
Add/remove ingredients from a recipe
Important Points to be included in the implementation
1.
Basic Django authentication can be used, but the GraphQL endpoints have to be allowed only for authenticated users. Do not implement login/signup web pages. We are okay to use createsuperuser management command to create a user. You may need to create a REST API endpoint to get the user’s signed-in access_token.
2.
Make sure that the code is clean and easy to read / understand.
3.
Make sure you use GraphQL (Graphene Django or Strawberry) for listing and mutations.
4.
Bonus points for using Django rest framework serializers with the GraphQL mutations.
Toolkit
Acme Inc. is very opinionated about their tech stack. The tools should be:
1. Framework: Django (Latest version)
2. Data storage – You can store the data anywhere you want; you can use Heroku PostgreSQL, or any other free PostgreSQL database on cloud.
3. All responses must be in json format.
•
Deploy the app in any free service such as Netlify, Heroku, etc and send us the link to the app (This is optional, but will get bonus points)
Feel free to contact me at arun.thomas@twistedmountainanimation.com for any queries.
