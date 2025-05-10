
# Currency Converter

## Description
This is a Spring Boot application that utilizes a public API to provide real-time currency conversion functionality.

## Features
- Fetch exchange rates for the specified base currency.
- Convert an amount between two currencies using the fetched exchange rates.

## Technologies Used
- Java 17
- Spring Boot
- Maven
- IDE (Preferred: Eclipse)

## Requirements
- Java 17
- Maven 3.9.9

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/nithulps/curency-converter.git
   ```

2. Move to the project folder:
   ```bash
   cd currency-converter
   ```

3. Checkout to the `master` branch:
   ```bash
   git checkout master
   ```

4. You need to log in to [Open Exchange Rates](https://openexchangerates.org/account).  
   - Create a new API key by visiting [this link](https://openexchangerates.org/account/app-ids).  
   - Copy the generated application key, as this will be required to fetch real-time currency data for the application.

## Building the Project
To build the project, run the following command:
```bash
mvn clean package -Dcurrency.api.key=<your-api-key>
```

## Running the Application
To run the application, use the following command:
```bash
java -jar -Dcurrency.api.key=<your-api-key> target/currencyconverter-0.0.1-SNAPSHOT.jar
```

Once the application is up and running, you can access it at:
```bash
http://localhost:8080/api/rates?base=USD
```

## API Documentation
API documentation is available at:
```bash
http://localhost:8080/swagger-ui/index.html
```
