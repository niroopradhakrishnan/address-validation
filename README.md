# Address validation

This utility program takes unformatted and/incomplete addresses from an Excel file and validates the address by calling a Google geocoding API. If the address is successfully validated, the formatted address along with the Google Place ID will be captured against each entry in an output Excel file. If the API returns any error, the error message is captured against each entry in an output file.

# How to use the utility

Before using the program, the following steps need to be completed:
1.	Install Python version 2.7 or above
2.	Install the required libraries of python using the command ‘pip install -r requirements.txt’
3.	Enable google map Geocoding API and generate an API key from https://console.developers.google.com/. There many costs associated to calling this API, please be aware and familiar with that.
4.	Copy and paste the API key into the program address_validation.py to replace the placeholder paste_api_key_here 
5.	Prepare an input file similar to address_input.xlsx in the repository. The first column is an ID and second column is unformatted address. You can have many ID & unformatted addresses as rows in the file
6.	Place the input file in a location and update the program with input address file location and name
7.	Update the program with output file desired name and location

After the above steps are completed, you can run the program using command ‘python address_validation.py’. Once the program displays message ‘Program completed!’, please check the output file in the location specified for the results.
