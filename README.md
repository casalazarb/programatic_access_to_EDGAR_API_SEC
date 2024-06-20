## SEC Filings Retriever
This code enables the retrieval of SEC filings, specifically 10-K and 10-Q documents, using the SEC EDGAR API. To use this tool, you need the type of document, the reporting date, and the company's ticker symbol.

## Features
Retrieve SEC 10-K and 10-Q documents programmatically.
Utilize the SEC EDGAR API for efficient document access.
Consolidate information into a DataFrame and save it as a CSV file.
Prerequisites
Python 3.x
requests library

## Functions
**fetch_cik(ticker, tickers_json)**
This function retrieves the Central Index Key (CIK) for a given company.

Parameters:

ticker (str): The ticker symbol of the company.
tickers_json (str): A JSON file downloaded from the SEC EDGAR API that maps company tickers to their CIKs.

Returns:

cik (str): The CIK that uniquely identifies the company in the SEC EDGAR system.

**get_document_url(cik, reporting_date)**
This function constructs the URL to access the desired SEC filing document.

Parameters:

cik (str): The CIK of the company.
reporting_date (str): The reporting date of the filing (end of the quarter for 10-Q documents and end of the year for 10-K documents).
Returns:

url (str): The URL where the document is located.
Output

The retrieved documents are in a htm file. All relevant information is consolidated into a DataFrame, which is then stored in a CSV file.

## Usage
This code was created to improve productivity in research projects involving mergers and acquisitions.

	
