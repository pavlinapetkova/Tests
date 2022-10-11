# Install Python

##### Step 1: Download the Python Installer binaries

- Open the official Python website in your web browser and navigate to the Downloads tab.
- Choose your operation system.
- Choose the Python 3.10 release.
- Click on the link to download the executable installer.

##### Step 2: Run the Executable Installer

- Once the installer is downloaded, run the Python installer.
- Check the Install launcher for all users check box. Further, you may check the Add Python 3.10 to path check box to include the interpreter in the execution path.
- Select Customize installation. Choose the optional features by checking the following check boxes:
-- Documentation
-- pip
-- tcl/tk and IDLE (to install tkinter and IDLE)
-- Python test suite (to install the standard library test suite of Python)
-- Install the global launcher for `.py` files. This makes it easier to start Python
-- Install for all users.
- Click Next. This takes you to Advanced Options available while installing Python. Here, select the Install for all users and Add Python to environment variables check boxes. Optionally, you can select the Associate files with Python, Create shortcuts for installed applications and other advanced options. Make note of the python installation directory displayed in this step. You would need it for the next step. After selecting the Advanced options, click Install to start installation.
- Once the installation is over, you will see a Python Setup Successful window.

##### Step 3: Add Python to environmental variables

- The last (optional) step in the installation process is to add Python Path to the System Environment variables. This step is done to access Python through the command line. In case you have added Python to environment variables while setting the Advanced options during the installation procedure, you can avoid this step.

##### Step 4: Verify the Python Installation

- You have now successfully installed Python 3.10. You can verify if the Python installation is successful either through the command line or through the IDLE app that gets installed along with the installation. Search for the command prompt and type “python”. You can see that Python 3.10 is successfully installed.
- An alternate way to reach python is to search for “Python” in the start menu and clicking on IDLE (Python 3.10).

# Install Playwright

- Install the Pytest plugin:

```python 
pip install pytest-playwright
```

- Install the required browsers:

``` python
playwright install
```

# Running Tests

- Open Terminal and find the directory of the test files.
- You can run a single test, a set of tests or all tests. Tests can be run on one browser or multiple browsers. By default tests are run in a headless manner meaning no browser window will be opened while running the tests and results will be seen in the terminal. If you prefer you can run your tests in headed mode by using the `--headed` flag.

- Running tests on Chromium

```python
pytest
```

- Running a single test file

```python 
pytest test_example.py
```

- Running tests in headed mode

```python
pytest --headed test_example.py
```

- Running Tests on specific browsers

```python
pytest test_example.py --browser firefox
```

- Running Tests on multiple browsers

```python
pytest test_example.py --browser firefox --browser webkit
```
