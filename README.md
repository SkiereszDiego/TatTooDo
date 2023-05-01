<details>
<summary>Elevator Pitch</summary>

 **PARA O(A)** proprietários de estúdios, gerentes e artistas  
 **QUE TEM** necessidade de gerenciar reservas, clientes, estoque e melhorando a eficiência e a satisfação do cliente  
 **O(A)** InkGEST  
 **E UM(A)** aplicação web para gerenciar especificamente estúdios de tatuagem   
 **QUE** melhora a eficiência do negócio, liberando mais tempo para os artistas se concentrarem em seu trabalho  
 **AO CONTRARIO DE** outros software de gerenciamento ele possui funcionalidades personalizadas para o mercado de estúdio de tatuagem.  
 **O PRODUTO** se destaca com o diferencial de um sistema de gift card exclusivo, aumentando a receita e a fidelidade do cliente.

 Pesquisa
 alem do discovery foi feito uma pesquisa no reddit e algumas coisas ficaram se destacando nos comentarios....
</details>

# Inkgest Tattoo Studio Management System
This is a web-based management system for a tattoo studio. It allows customers to register, view available products, and make appointments, while also providing staff with tools for managing inventory, scheduling appointments, and more.

## Getting Started
<details>
<summary>Click to expand</summary>

### Prerequisites
- Node.js
- MongoDB

### Installation
1. Clone the repo

``` 
    git clone  https://github.com/SkiereszDiego/InkGest.git
```

2. Install NPM packages in the root and client directories
``` 
    cd inkgest
    npm install
    cd client
    npm install
``` 
3. Create a .env file in the root directory and add the following variables
``` 
    MONGO_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
``` 
4. Start the application
``` 
    npm run dev
``` 
This will start the server and client applications concurrently.

</details>

## Project Structure
<details>
<summary>Click to expand</summary>
The project is organized into separate directories for the frontend and backend applications. <br>
Here's a breakdown of the project structure:

```
inkgest/
├── client/
│   ├── public/
│   │   ├── index.html            
│   │   └── ...
│   ├── src/
│   │   ├── components/
│   │   │   ├── Login.js          
│   │   │   ├── SignUp.js         
│   │   │   ├── Home.js
│   │   │   ├── UserList.js
│   │   │   ├── ProductList.js        
│   │   │   ├── GiftCards.js      
│   │   │   ├── PurchaseCard.js   
│   │   │   └── RedeemCard.js    
│   │   ├── App.js                
│   │   └── ...
├── server/
│   ├── config/                  
│   │   ├── db.js                
│   │   ├── jwt.js    
│   ├── controllers/
│   │   ├── auth.js              
│   │   ├── giftCards.js         
│   │   └── users.js 
│   ├── middleware/              
│   │   ├── auth.js  
│   ├── models/
│   │   ├── giftCard.js          
│   │   └── user.js   
│   ├── routes/
│   │   ├── auth.js              
│   │   ├── giftCards.js         
│   │   ├── users.js     
│   ├── index.js
│   ├── package.json
│   └── ...
├── tests/                        
│   ├── giftCards.test.js        
│   ├── payments.test.js         
│   └── users.test.js  
├── .env
└── ...
```

### Frontend
The frontend is built using ??React?? and is located in the client directory. The directory structure is as follows:

- public/: contains the index.html file and other public assets
- src/: contains the React components and application logic
    - components/: contains the reusable React components used throughout the application
    - App.js: the root component of the application

### Backend
The backend is built using Node.js and Express, and communicates with the MongoDB database using Mongoose. The directory structure is as follows:

- controllers/: contains the controllers that handle requests and responses
- models/: contains the Mongoose models for the MongoDB collections
- routes/: contains the Express routes for the API endpoints
- index.js: the main entry point for the backend application
</details>

## Features
<details>
<summary>Click to expand</summary>

### Customer Registration
Customers can register for an account and view their account information, including their appointment history and any products they've purchased.

### Product Registration
Staff can add new products to the system, including information about the product, such as name, price, and quantity on hand.

### User Registration
Staff can create new user accounts, assign roles and permissions, and manage user accounts.

### Inventory Control
Staff can manage the inventory of products, including viewing product information, adding new products, and updating product information.

### Gift Card System
Customers can purchase gift cards, which can be redeemed for products or services at the studio. Staff can view gift card balances and redeem gift cards as payment for appointments and purchases.

</details>

## License
This project is licensed under the MIT License - see the LICENSE file for details.
