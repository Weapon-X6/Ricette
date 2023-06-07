# Ricette
A RESTful API to handle recipes

### Features

* Allows listing/adding/updating/deleting recipes, ingredients and tags
* Uses JSON Web Tokens

### Up & Running
Just run
```
docker-compose up -d --build
```
Then create a superuser to be able to use the endpoints
```
docker-compose exec app python manage.py createsuperuser
```

Finally: 

1. Access the API at http://127.0.0.1:8000/api/docs/ and make call to /api/user/token/ providing your newly created credentials
2. Copy the value of token within your response body
3. Scroll to the top and click on Authorize, in tokenAuth enter `Token {YourCopiedToken}`, click authorize, and your done!


