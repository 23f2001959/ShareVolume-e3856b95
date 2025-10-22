# Project Name: ShareVolume

## Summary:
This project fetches data from the SEC API for a specific company (Broadridge Financial Solutions in this case) and calculates the maximum and minimum common stock shares outstanding values for fiscal years after 2020. It then displays this information in a visually appealing HTML page.

## Setup:
1. Clone the GitHub repository: `git clone https://github.com/yourusername/ShareVolume.git`
2. Navigate to the project directory: `cd ShareVolume`

## Usage:
1. Open the `index.html` file in a web browser to view the ShareVolume information for Broadridge Financial Solutions.
2. To view ShareVolume information for a different company based on CIK, add `?CIK=[10-digit CIK]` to the URL in the browser (e.g., `index.html?CIK=0001018724`).

## Code Explanation:
1. The project fetches data from the SEC API using a descriptive User-Agent as per SEC guidance.
2. It reads the fetched JSON data, filters shares entries for fiscal years after 2020 with numeric values, and saves the processed data in `data.json`.
3. It dynamically renders an `index.html` page with the company name, maximum and minimum share values, and fiscal years without reloading the page.
4. It supports the `?CIK=` query parameter to fetch data for alternate companies.

## License:
This project is licensed under the MIT License. See the LICENSE file for more details.