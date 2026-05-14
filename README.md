# mizuyokan

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A web map of "mizuyokan" (a traditional Japanese winter confection) shops in Fukui Prefecture, Japan. This project visualizes shop data from 2011.

## Demo

**Live Application: [https://code4fukui.github.io/mizuyokan/](https://code4fukui.github.io/mizuyokan/)**

The user interface displays an interactive map with pins marking shop locations. Clicking a pin reveals a popup with the shop's name, address, phone number, price, and a photo of its mizuyokan. A filterable, sortable table of all shop data is shown alongside the map.

## Features

-   **Interactive Map**: Displays all mizuyokan shop locations from the dataset.
-   **Detailed Information**: Each map marker provides shop details, including photos.
-   **Data Table**: A `csv-viewer` component presents the raw data in a user-friendly table.
-   **Static Site**: Runs entirely in the browser with no server-side backend required.
-   **Legacy Version**: Includes an older implementation (`index-old-googlemaps-ver.html`) using the Google Maps API.

## How It Works

This project is a static HTML page that uses modern web components to display data:

-   `<csv-map>`: Renders the interactive map and markers directly from the `fukui-mizuyokan.csv` file.
-   `<csv-viewer>`: Renders the data table from the same CSV file.

These components are imported from their respective repositories and require no local installation or build step.

## Data

The shop information is stored in [`fukui-mizuyokan.csv`](fukui-mizuyokan.csv). The data is from 2011 and includes the following columns:

-   `店舗名` (Shop Name)
-   `電話番号` (Phone Number)
-   `住所` (Address)
-   `緯度` (Latitude)
-   `経度` (Longitude)
-   `写真URL` (Photo URL)
-   `価格` (Price)

## Usage

To run this project locally, simply open the `index.html` file in a web browser.

## Credits

This application was created by Taisuke Fukuno.

-   **Author**: [Taisuke Fukuno (福野泰介)](https://fukuno.jig.jp/)
-   **Twitter**: [@taisukef](https://twitter.com/taisukef)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.