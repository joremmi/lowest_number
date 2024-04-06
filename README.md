# Find the Lowest Number in a File

This repository contains a Python script designed to identify and write the lowest number from a given input file to a specified output file. It demonstrates the use of basic Python programming concepts and file handling operations. Additionally, this project is integrated with GitHub Actions to automate the testing of the script across different scenarios via a CI/CD pipeline.

## Usage

To run the script, you will need Python 3 installed on your system. The script can be executed with the following command:

```
python find_lowest_number.py <input_file> <output_file>
```

or, if your system is configured to use Python 3 by default:

```
python3 find_lowest_number.py <input_file> <output_file>
```

**Example:**

```
python3 find_lowest_number.py numbers.txt lowest_number.txt
```

This will read the numbers from `numbers.txt`, find the lowest number, and write it to `lowest_number.txt`.

### Prerequisites

1. **Python 3 Installation:** Ensure Python 3 is installed on your system. You can download it from the [official Python website](https://www.python.org/).

## Automated Testing with GitHub Actions

This repository utilizes GitHub Actions to automate the testing of the `find_lowest_number.py` script. The CI/CD pipeline is triggered on every push to the repository, executing tests to verify the script's functionality across three predefined cases:

1. **Multiple Numbers:** Verifies the script correctly identifies the lowest number in a file containing multiple numbers.
2. **Single Number:** Tests the script's ability to handle a file with only one number.
3. **Blank File:** Ensures the script outputs the correct message when provided with an empty file.

The test inputs and expected outputs are located in the `test_data` directory. The GitHub Actions workflow is defined in `.github/workflows/python-app-test.yml`, detailing each step taken to set up the environment, run the tests, and validate the outputs against the expected results.

## Contributing

We welcome contributions to this project! If you have suggestions to improve the script or the testing pipeline, please feel free to fork this repository, make your changes, and submit a pull request.
