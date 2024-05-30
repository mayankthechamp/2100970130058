![E-commerce 1](https://github.com/mayankthechamp/2100970130058/assets/99077491/0f1217c5-639b-4f35-b7ae-e03aba0489b6)

Hello this is a E-commerce App based on React.js 

### Top Products HTTP Microservice

This project implements a microservice that fetches and displays top products from multiple e-commerce companies. The microservice exposes two REST APIs: one for retrieving the top products within a category and another for fetching details of a specific product.

#### Features:
- **Get Top N Products:** Allows users to retrieve the top N products within a specified category and price range. Supports sorting based on price, rating, and discount, with pagination for results exceeding 10 items.
- **Get Product Details:** Provides detailed information about a specific product, including its name, price, rating, discount, and availability.

#### Technologies Used:
- **Node.js:** Backend server environment.
- **Express:** Web framework for Node.js used to create RESTful APIs.
- **Axios:** HTTP client for making requests to external APIs.
- **REST APIs:** Follows RESTful principles for resource management.
-
-

#### Setup Instructions:
1. Clone the repository.
2. Install dependencies using `npm install`.
3. Run the server using `npm start`.
4. Access the APIs at the specified endpoints (`/categories/:category/products` and `/categories/:category/products/:productid`).

#### API Endpoints:
- `GET /categories/:category/products`: Retrieves the top N products within a category.
  - Query Parameters:
    - `n`: Number of products to retrieve.
    - `page` (optional): Page number for pagination.
    - `minPrice` (optional): Minimum price filter.
    - `maxPrice` (optional): Maximum price filter.
    - `sort` (optional): Sort parameter (price, rating, discount).
    - `order` (optional): Sort order (asc, desc).

- `GET /categories/:category/products/:productid`: Retrieves details of a specific product by ID.

#### Additional Information:
- **Caching:** The microservice caches product data to improve performance and reduce external API calls.
- **Access Token:** Uses an access token to authenticate requests to external APIs.
- **Error Handling:** Implements error handling for failed API requests and invalid parameters.
- **Logging:** Logs important events and data for debugging and monitoring purposes.

#### Disclaimer:
- The product data is subject to change by the e-commerce companies, and the microservice may not always reflect real-time information.

