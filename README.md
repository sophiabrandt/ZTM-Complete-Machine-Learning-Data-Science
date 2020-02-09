[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science">
    <img src="logo.png" alt="Logo">
  </a>

  <h3 align="center">ZTM -  Complete Machine Learning and Data Science</h3>

  <p align="center">
    Code repository for Udemy course
    <br />
    <a href="https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science">View Demo</a>
    ·
    <a href="https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/issues">Report a Bug</a>
    ·
    <a href="https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/issues">Request Feature</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About the Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

The repository contains my code for the **[Complete Machine Learning and Data Science: Zero to Mastery][ztm]** Udemy course.

See the [original course materials by Daniel Bourke][origrepo].

You can read my thoughts, lecture notes, and observations on my blog:

- [A Walkthrough of the “Complete Machine Learning and Data Science: Zero to Mastery” Course (Part 01)](https://www.rockyourcode.com/a-walkthrough-of-the-complete-machine-learning-and-data-science-zero-to-mastery-course-part-01/)
- [A Walkthrough of the “Complete Machine Learning and Data Science: Zero to Mastery” Course (Part 02)](https://www.rockyourcode.com/a-walkthrough-of-the-complete-machine-learning-and-data-science-zero-to-mastery-course-part-02/)

The project setup with Docker and docker-compose is heavily influenced by the [Data Science Docker Template](https://github.com/caesarnine/data-science-docker-template) by Binal Patel.

### Built With

- [Docker](https://www.docker.com/) and docker-compose
- Python
- [Jupyter Notebooks](https://jupyter.org/)

<!-- GETTING STARTED -->

## Getting Started

To get a local copy up and running follow these steps:

### Prerequisites

You'll need Docker and docker-compose:

- Docker

```sh
docker --version
> Docker version 19.03.5-ce
```

- docker-compose

```sh
docker-compose -v
> docker-compose version 1.25.3
```

### Installation

1. Clone the repo

```sh
git clone https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.git
```

2. Create `.env_dev` file with the following format:

```
# credentials and database information
db_username=test_username
db_password=test_password
db_host=test_host
db_port=test_port
db_name=test

# disables lag in stdout/stderr output
PYTHONUNBUFFERED=1
PYTHONDONTWRITEBYTECODE=1

# random seed
random_seed=42
```

3. Build and run container

```sh
docker-compose up --build -d
```

<!-- USAGE EXAMPLES -->

## Usage

1. Go to `http://localhost:8888` for JupyterLab. Enter access token: `local_dev`.

2. Develop and save any notebooks into `/notebooks`. Save final artifacts/models needed for production in `/code`.

<!-- ROADMAP -->

## Roadmap

See the [open issues](https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->

## License

Distributed under the MIT License. See [`LICENSE`](LICENSE.txt) for more information.  
Original code by Andreie Neagoie, Daniel Bourke. Original Docker setup by Binal Patel.

<!-- CONTACT -->

## Contact

Sophia Brandt - [@hisophiabrandt](https://twitter.com/hisophiabrandt)

Project Link: [https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science](https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science)

<!-- ACKNOWLEDGEMENTS -->

## Acknowledgements

- [Complete Machine Learning and Data Science: Zero to Mastery][ztm] by Andrei Neagoie & Daniel Bourke
- [Data Science Docker Template](https://github.com/caesarnine/data-science-docker-template) by Binal Patel

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.svg?style=flat-square
[contributors-url]: https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.svg?style=flat-square
[forks-url]: https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/network/members
[stars-shield]: https://img.shields.io/github/stars/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.svg?style=flat-square
[stars-url]: https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/stargazers
[issues-shield]: https://img.shields.io/github/issues/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.svg?style=flat-square
[issues-url]: https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/issues
[license-shield]: https://img.shields.io/github/license/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science.svg?style=flat-square
[license-url]: https://github.com/sophiabrandt/ZTM-Complete-Machine-Learning-Data-Science/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png
[ztm]: https://www.udemy.com/course/complete-machine-learning-and-data-science-zero-to-mastery/
[origrepo]: https://github.com/mrdbourke/zero-to-mastery-ml
