# ShareVolume 

ShareVolume is a project that fetches and displays the number of outstanding shares of a company, specifically Amazon (AMZN), from the SEC's XBRL API. It filters for entries whose fiscal year (fy) is greater than 2020 and includes a numeric value (val). The project saves the data in a structured JSON format and renders an appealing HTML page displaying the entity's name and the highest and lowest val figures.

## Features

1. **API Interaction**: Fetches data from the SEC's XBRL API for a specific Central Index Key (CIK), in this case, Amazon's CIK.
2. **Data Filtering**: Filters the fetched data for entries whose fy is greater than 2020 and includes a numeric val.
3. **Data Structuring**: Structures the filtered data into a specific JSON format.
4. **Data Rendering**: Renders a visually appealing HTML page displaying the entity's name and the highest and lowest val figures.
5. **Live Updates**: Updates the HTML page's content without reloading when opened with a different CIK in the URL.

## Setup Instructions

1. Clone the repository: `git clone https://github.com/aswego123/ShareVolume.git`
2. Navigate to the project directory: `cd ShareVolume`

## Usage Instructions

1. Open the `index.html` file in your web browser.
2. To see information for a different CIK, append `?CIK=<10-digit-CIK>` to the URL.

## Technical Implementation

The project primarily uses JavaScript to interact with the SEC's XBRL API and fetch data for a specific CIK. It then filters the data for entries with a fy greater than 2020 and a numeric val, structures it into a specific JSON format, and saves it. The project uses HTML and CSS to render an appealing page that displays the fetched data. The project also uses JavaScript's Fetch API to update the page's content live when opened with a different CIK in the URL.

## License Information

ShareVolume is licensed under the terms of the MIT license.

## Live Demo

You can check out the live demo of the project [here](https://aswego123.github.io/ShareVolume/).