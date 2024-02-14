# STRK Drop Checker

This script checks for eligible wallets for the $STRK drop against a list of your wallets. It reads wallet addresses from a text file, compares them with a list of eligible wallets from JSON files, and outputs the total $STRK drop amount you are eligible for along with the eligible wallet addresses.

## Prerequisites

Before running the script, ensure you have Python installed on your system. This script was developed with Python 3.8.5.

## Setup

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Ensure you have a `wallets.txt` file in the project directory with your wallet addresses listed, one per line. Each address should start with `0x`.

## Running the Script with Docker

To build and run the script using Docker, follow these steps:

1. Build the Docker image: `docker-compose build`
2. Run the script inside a Docker container: `docker-compose up`
   
This will use the `wallets.txt` file from your project directory as a volume in the Docker container.

## Running the Script

To run the script, execute the following command in your terminal:

```bash
python main.py
```

## Output

The script will print the eligible wallet addresses and their corresponding $STRK drop amounts to the console. Additionally, it will generate a `eligble_wallets.json` file in the project directory containing the list of eligible wallets.

## Contributing

Contributions are welcome! If you have suggestions for improving the script, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.