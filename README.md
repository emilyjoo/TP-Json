Product Showcase
This project is a simple product showcase web page that displays a list of products with their variations in size and color. The data for the products is embedded directly into the HTML file as a JavaScript array.

File
products.html: The main HTML file that contains the structure and logic for displaying the products.
Structure
HTML
The HTML file includes the following sections:

Head Section: Includes meta tags, Bootstrap
CSS for styling, and custom styles for the product cards.
Body Section: Contains a hidden template for product cards and a container for displaying the product cards.
JavaScript
The JavaScript code embedded in the HTML file performs the following tasks:

Embed Product Data: The product data is embedded directly into the script as a JavaScript array.
Render Products: The script iterates over the product data and creates a card for each product using a hidden template.
Dynamic Variations: For each product, the script dynamically adds color and size options based on the available variations.
Update Price and Stock: When a user selects a color and size, the script updates the displayed price and stock information for the selected variation.
Usage
To use this project, simply open the products.html file in a web browser. The page will display a list of products with their variations in size and color. Users can select different colors and sizes to see the corresponding price and stock information.

Customization
You can customize the product data by modifying the JavaScript array embedded in the products.html file. The structure of the array should match the following format:
const produits = [
  {
    "_id": "P001",
    "nom": "Product Name",
    "description": "Product Description",
    "image": "Product Image URL",
    "categorie": {
      "_id": "C001",
      "nom": "Category Name"
    },
    "variations": [
     {
        "taille": "Size",
        "couleur": { "nom": "Color Name", "code": "Color Code" },
        "quantiteEnStock": Stock Quantity,
        "prix": Price,
        "image": "Variation Image URL"
      }
    ]
  }
];

Dependencies
Bootstrap for styling.
