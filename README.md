# osmosis-tick-price

# Osmosis Pool Tick Price Calculator

This is a simple web page that calculates the price for a given tick in an Osmosis liquidity pool. If no tick is provided, it uses the current tick of the pool.

## Features

- Enter a pool ID to interact with a specific Osmosis pool.
- Specify a tick to calculate the price for that tick, or leave it blank to use the pool's current tick.
- Basic error handling for API responses.

## How to Use

1. **Set Up**: 
   - Clone or download this repository.
   - Open the `index.html` file in your browser.

2. **Usage**:
   - Enter the **Pool ID** of the Osmosis pool you're interested in.
   - Optionally, enter a specific **Tick** number. If left blank, the current pool tick will be used.
   - Click on "Get Price" to see the calculated price.

## Key Points

- **Endpoint**: Replace `YOUR_OSMOSIS_RPC_ENDPOINT` in the JavaScript with an actual Osmosis RPC endpoint. You can use a public node or run your own.

- **Query**: The code includes a placeholder for querying Osmosis. You might need to adjust this based on the actual API endpoints or contract interactions for fetching pool information.

- **Error Handling**: Basic error handling is implemented. Enhance this for production use to provide more detailed user feedback.

- **UI**: The provided UI is very basic. Consider enhancing it or using a framework for better user interaction.

- **JavaScript**: Utilizes `BigInt` for accurate calculations with large numbers, which is crucial for blockchain applications.

## Setup

- You need a web server to run this HTML file properly due to CORS issues with fetching data from external APIs directly from the file system. You can use Node.js with `http-server`, Python's `http.server`, or any other local server:
  - Using `http-server`: 
    ```sh
    npm install -g http-server
    cd path/to/your/project
    http-server
    ```
  - Using Python:
    ```sh
    python3 -m http.server  # Python 3
    python -m SimpleHTTPServer 8000  # Python 2
    ```

## Limitations

- This project assumes the availability and stability of the Osmosis blockchain's API. Performance might degrade if the network is under heavy load or if endpoints are changed.

- The calculation of price from tick might not be 100% accurate due to simplifications in the JavaScript implementation compared to actual blockchain logic.

## Contributing

Feel free to fork this project, make changes, and submit pull requests:

- Fix bugs.
- Enhance UI/UX.
- Improve API interaction for better reliability and error handling.

## License

[Choose a license or add your own]
