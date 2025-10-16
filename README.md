# Sales Summary Application

This is a single-page web application that:
1. Fetches sales data from a CSV file
2. Calculates the total sales amount
3. Displays the result in a Bootstrap-styled interface
4. Sets the page title to a specific value as required

## Implementation Details

- Uses Bootstrap 5 from jsDelivr CDN for styling
- Fetches CSV data from a base64-encoded data URI
- Processes the CSV data client-side to calculate total sales
- Displays the result in the element with id `total-sales`
- Sets the document title as specified in the requirements

## How It Works

1. On page load, the application fetches the CSV data from the embedded data URI
2. The CSV is parsed line by line, skipping the header row
3. Sales values are extracted from the second column and added to a running total
4. The total is displayed formatted as currency in the card element

## Error Handling

If there's an error fetching or processing the data, an error message will be shown in place of the total.

## Requirements Verification

- [x] Document title is set correctly
- [x] Bootstrap 5 is loaded from jsDelivr
- [x] Total sales are calculated and displayed in #total-sales element
- [x] Base64 data URI is used as provided without modification