# CSV Analyzer

This project provides a web application for analyzing CSV files using Langchain and Panel. It allows users to:

*   Upload and visualize CSV data.
*   Ask questions about the data using a language model.
*   Generate custom plots.

The main components are:

*   **Data Loading and Display:** Uses `pandas` to read CSV files and `panel.widgets.Tabulator` to display the data in an interactive table.
*   **Interactive Plotting:** Employs `plotly.express` for creating scatter plots with customizable X and Y axes.
*   **Language Model Integration:** Leverages `langchain` and `OpenAI` to create a CSV agent that can answer questions about the data.
*   **User Interface:** Built with `panel`, providing widgets for file input, text input, buttons, and chat display.

## How to Download the GitHub Repository

To download the project, use the following command:

```bash
git clone https://github.com/dpalominop/query-csv-files.git
cd query-csv-files
```

## How to Setup the Virtual Env Using the Requirements File

1. Create a virtual environment:
```bash
python3 -m venv .venv
```
2. Activate the virtual environment:
```bash
source .venv/bin/activate
```
3. Install the required packages:
```bash
pip install -r requirements.txt
```
## How to Run the Project
1. Ensure you have set up your `.env` file with the OPENAI_API_KEY.

2. Run the Jupyter Notebook:
`jupyter notebook csv-analyzer.ipynb`
Or if you are using VS Code, simply open the `csv-analyzer.ipynb` file and run the cells.

3. Uncomment and run the following line in the notebook to start the web application:
`template.show(open=False, address='0.0.0.0', port=5006, websocket_origin=url)`

**Note:** You may need to adjust the address, port, and websocket_origin parameters as needed.
