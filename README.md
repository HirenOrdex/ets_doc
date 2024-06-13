# Swagger Comments Generator

## Overview

This script generates Swagger comments in a specific format for API endpoints defined in JSON files. It helps maintain consistency and clarity in documenting API endpoints using Swagger/OpenAPI specifications.

## Features

- Automatically reads Swagger/OpenAPI JSON files from a specified folder.
- Generates structured Swagger comment blocks for each endpoint, including tags, summary, parameters, request body, and responses.
- Handles nested properties and arrays in request bodies and parameters.
- Outputs generated Swagger comments to separate `.txt` files for each Swagger JSON file processed.
- Compatible with Google Colab for cloud-based execution.

## Requirements

- Python 3.x
- JSON formatted Swagger/OpenAPI specification files in a specified folder

## Usage in Google Colab

1. Upload your Swagger/OpenAPI JSON files to Google Colab's virtual machine:
   - Use the file upload feature in Google Colab to upload your JSON files.
   ```python
   from google.colab import files
   uploaded = files.upload()

## Notes

- Ensure the structure and format of your JSON files adhere to Swagger/OpenAPI specifications for proper merging and compatibility.
- This script assumes all JSON files in the 'api' folder are valid Swagger/OpenAPI documents.

## Troubleshooting

- **No JSON Files Found**: If the script reports no JSON files found in the 'api' folder, ensure your files are uploaded and the path is correct.
## Resources for @swaggger 

[Access to Google Colab or Jupyter Notebook environment. file](https://github.com/HirenOrdex/ets_doc/blob/main/_swagger_main.ipynb)


[chatGPT Promt](https://chatgpt.com/share/64245474-b90b-414b-a3e8-7fa5e1a8341c)

[video doc](https://photos.app.goo.gl/K1QvQVNvRrWjK4cw7)
