# GOV.UK-flask-skeleton

This is a template project for building frontends using the gov.uk toolkit using flask.

### Contents

- [Usage](#usage)
- [Getting Started](#getting-started)
- [Acceptance Tests](#acceptance-tests)
- [Code Style Checking](#code-style-checking)

## Usage

```
get     /helloworld                 # test endpoint for the app
```

## Getting Started
1. Clone the repo

2. Get the GOV.UK toolkit submodule
    ```
    git submodule update --init
    ```

3. In the directory enter the command
    ```
    pip install -r requirements.txt
    ```

4. To run the application run the command
    ```
    python run.py runserver
    ```
    
## Acceptance Tests

- Standard way
```
./acceptance-tests/run_tests.sh
```

- Cut down version of output
```
./acceptance-tests/run_tests.sh --format progress
```

- Only run test with specific tag
```
./acceptance-tests/run_tests.sh --tags @USXX
```

### Code Style Checking

1. App

    ```
    flake8 .
    ```
    > Requires flake8, install with ```pip install flake8```

2. Acceptance tests
    
    ```
    ./acceptance-tests/run_linting.sh
    ```
