# FakeBuster

## Description
FakeBuster is a decentralized application that uses QR codes to store product details. These details are stored in blocks of data, ensuring that the data cannot be modified. This approach maintains the transparency of the supply chain.

### Data Flow
![Data Flow](https://imgur.com/VGIPtDU.png)

### Why blockchain? <a name="why_blockchain"></a>
+ Unlike a normal database, Blockchain has a non-destructive (immutable) way to track data changes over time. This means that data is not editable rather, whenever updates are made, a new block is added to the “block-chain”. This helps track historical data (authenticity and owner data) of a product.
+ Given the amount of data to be dealt with (large amount of products being developed), if you have to keep track of all of them, it is better to have a decentralized and distributed network of nodes so that no entity can tamper with the product data and we also obtain 100% up time.
+ Transparent nature of the Blockchain helps avoid [parallel trade](https://en.wikipedia.org/wiki/Parallel_import).
+ Using Blockchain, authenticity can be checked and ownership of a product can be transferred _decades_ from now; even if the product is discontinued.

## Features
- **Decentralized Storage:** Data is stored in a decentralized manner, ensuring security and immutability.
- **QR Code Integration:** Each product is associated with a QR code that stores its details.
- **Supply Chain Transparency:** The system ensures transparency in the supply chain by preventing data modification.
- **User-friendly Interface:** Easy-to-use interface for adding and retrieving product details.
- **Secure:** Utilizes blockchain technology to ensure data integrity and security.
- **Scalable:** Designed to handle a large number of products and transactions efficiently.

## Installation
To install and run FakeBuster locally, follow these steps:
1. **Clone the repository:**
    ```bash
    git clone https://github.com/priyanshix/FakeBuster.git
    ```

2. **Navigate to the project directory:**
    ```bash
    cd FakeBuster
    ```

3. **Set up XAMPP:**
    - Download and install [XAMPP](https://www.apachefriends.org/index.html).
    - Start the Apache and MySQL services from the XAMPP control panel.

4. **Configure the database:**
    - Open your web browser and go to `http://localhost/phpmyadmin`.
    - Create a new database named `fakebuster`.
    - Import the database schema from the `database` folder in the project directory into the `fakebuster` database.

5. **Move the project to the XAMPP directory:**
    - Copy the project files to the `htdocs` directory in your XAMPP installation folder. Typically, this would be `C:/xampp/htdocs/`.

6. **Update the database configuration:**
    - Open the `config.php` file in the project directory.
    - Update the database connection settings to match your XAMPP setup:
      ```php
      <?php
      $servername = "localhost";
      $username = "root";
      $password = "";
      $dbname = "fakebuster";
      ?>
      ```

## Usage
1. **Start the application:**
    - Open your web browser and navigate to `http://localhost/FakeBuster`.

2. **Access the application:**
    - Use the provided interface to add and retrieve product details using QR codes.

