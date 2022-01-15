# Shopify Backend Application Summer 2022

# Usage
    1. Install dependencies using:
        npm install
        
    2. Run in dev mode using:
        npm run dev
        If PortNumber is already in use, you can change it in server.js line 25.

    3. Use an app like Postman to view data (If port number was changed, enter changed portnumber in below links.)
    
    - To View All Products, send GET request to http://localhost:4000/api/products.

    - To Filter Product by ID, simply send a GET request to http://localhost:4000/api/products/<ID Number>. For eg, if you want to view product with ID = 1, navigate to http://localhost:4000/api/products/1 .

    - To Insert Product, send a POST request to http://localhost:4000/api/products with the item details in the Body in a JSON format. It will create a new product with a uuid.
        Example:
        {
        "name" : New Product
        "description" : "This is a new product",
        "price": 100
        }

    - To Edit a Product, send a PUT request to http://localhost:4000/api/products/<id of product you want to edit> with new items details in the Body in a JSON format.
        Example: 
        {
        "name" : "Updated title",
        "description" : "This is an updated product",
        "price": 100
        }

    - To Delete a Product, send a DELETE request to http://localhost:4000/api/products/<id of product you want to delete>.
