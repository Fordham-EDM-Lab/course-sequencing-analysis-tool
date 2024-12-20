# seq_tool

The **seq_tool** is a Python package that implements the Generalized Sequential Pattern (GSP) algorithm. Originally developed as part of the Course Sequencing Analysis Tool (CSAT) to analyze and sequence student course data, the toolkit has been extended to support more generalized use cases. It is designed for applications where analyzing sequential patterns is essential, such as course sequencing or other data patterns.

The package supports grouping items based on a specified granularity using concurrency and provides both a command-line interface (CLI) and a graphical user interface (GUI).

## Features

- **GSP Algorithm**: Analyze sequential patterns using the Generalized Sequential Pattern (GSP) algorithm.
- **Granularity-Based Grouping**: Use concurrency to group items by a specified time granularity, such as semesters (quarters) or months.
- **Command-Line Interface**: Run the GSP algorithm from the terminal for efficient scripting and automation.
- **Graphical User Interface**: Easily configure and run the algorithm using an interactive graphical interface.

## Installation

Install from command-line via PyPi project:
```bash
pip install seq-tool
```

## Usage

### Command-Line Interface

You can run the GSP algorithm using the CLI. Here’s an example:

```bash
seq-cli -i data.csv -s 50,100 -c BIO,CHEM --mode separate -o results --concurrency
```

For more detailed instructions and examples, please refer to the [CSAT Manual](https://drive.google.com/file/d/1Mt1-W6ZfwCeUzJdNsK4tcwasUU9xYLC0/view).

### Graphical User Interface

Launch the GUI for an easy-to-use interface:

```bash
seq-gui
```

The GUI allows you to:
- Load your data file.
- Set support thresholds and categories.
- Group items based on granularity (e.g., semester or month).

## Requirements

- Python 3.10 or later
- Dependencies are automatically installed when you run `pip install seq-tool`.

## Data Requirements

To understand the required data format, refer to the [Data Dictionary](https://docs.google.com/spreadsheets/d/19fIA5eiZxCav0MiElDoTDvuyinyYroxuJF9LWmQxvNc/edit?usp=sharing).

### Example Datasets

Example datasets for testing and exploring the CSAT are available [here on Google Drive](https://drive.google.com/drive/folders/1hyjKf69IY1wbkWwSl0AzG-wJTITOXlIW?usp=sharing).

## Development Roadmap

- **Current**: Exploring runtime. Potentially find ways to optimize the algorithm to improve performance for large datasets, such as parallel execution.
- **Future**: Determining how to include the time (span?) to better understand the output.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
