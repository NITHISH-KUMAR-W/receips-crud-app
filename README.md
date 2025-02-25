// README.md
# Recipes App

This is a CRUD API for managing recipes using Node.js, Express.js, and MongoDB.

## Installation
1. Clone the repository
2. Install dependencies: `npm install`
3. Create a `.env` file and add your MongoDB URI
4. Run the server: `npm start`

## API Endpoints
### Base URL: `https://receips-crud-app.onrender.com`

#### Create a new recipe
`POST /api/recipes`
```json
{
  "title": "Chicken Biriyani",
  "ingredients": ["Chicken", "Basmati Rice", "Yogurt", "Onions", "Tomatoes", "Spices", "Cilantro"],
  "instructions": "Marinate chicken with yogurt and spices. Cook onions and tomatoes, add marinated chicken. Layer with cooked rice and cook on low heat.",
  "category": "Indian"
}
```

#### Retrieve all recipes
`GET /api/recipes`

#### Retrieve a single recipe
`GET /api/recipes/{id}`

#### Update a recipe
`PUT /api/recipes/{id}`
```json
{
  "title": "Updated Pasta Carbonara",
  "ingredients": ["Pasta", "Eggs", "Bacon", "Cheese", "Black Pepper"],
  "instructions": "Cook pasta, mix all ingredients, serve warm.",
  "category": "Italian"
}
```

#### Delete a recipe
`DELETE /api/recipes/{id}`