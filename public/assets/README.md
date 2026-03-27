"""
api-service README
================

Table of Contents
-----------------

* [Overview](#overview)
* [Getting Started](#getting-started)
* [Usage](#usage)
* [API Documentation](#api-documentation)
* [Contributing](#contributing)
* [License](#license)
* [Acknowledgements](#acknowledgements)
"""

import os

def get_project_root():
    return os.path.dirname(os.path.abspath(__file__))

def get_api_spec():
    return os.path.join(get_project_root(), 'api_spec.json')

def get_example_usage():
    return """
    # Example Usage
    from api_service import APIClient

    client = APIClient()
    response = client.get('/users')
    print(response.json())
    """

def get_api_documentation():
    return """
    # API Documentation
    This API has the following endpoints:

    * `GET /users`: Retrieve a list of users
    * `POST /users`: Create a new user
    """

def get_contributing_guidelines():
    return """
    # Contributing
    Contributions are welcome! Please fork the repository and submit a pull request.
    """

def get_license():
    return """
    # License
    MIT License
    Copyright (c) [Year] [Author]
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.
    """

def get_acknowledgements():
    return """
    # Acknowledgements
    This project was made possible by [Contributors].
    """

if __name__ == '__main__':
    print(get_project_root())
    print(get_api_spec())
    print(get_example_usage())
    print(get_api_documentation())
    print(get_contributing_guidelines())
    print(get_license())
    print(get_acknowledgements())