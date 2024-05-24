# Python Environment Management Tools Overview

## 1. virtualenv
- **Recommendation:** Only suitable if you're still working with Python 2.
- **Description:** virtualenv is an older tool primarily used for Python 2 environments.

## 2. venv
- **Advantage:** Simple to use.
- **Disadvantages:** 
  - Limited functionality; can only create virtual environments.
  - Unable to specify system-wide Python versions.
  - Lacks management of existing environments, such as selecting from a list of previously created ones.
  - Default location for virtual environments within project folders can clutter project management.

## 3. pipenv
- **Creator:** Kenneth Reitz, author of requests library.
- **Stability:** Unstable; may produce inconsistent results.
- **Issues:** 
  - Repetitive installations may yield different outcomes.
  - Despite promises, does not effectively resolve package versioning issues.

## 4. anaconda / conda
- **Recommendation:** Initially suggested for beginners in scientific computing.
- **Issues:** 
  - Bulky installation, occupying significant disk space.
  - miniconda, a lightweight version, still exhibits aggressive dependency installation behavior.
  - Dependency discrepancies between "conda list" and "pip list".

## 5. poetry
- **Advantage:** Considered the superior choice.
- **Description:** Utilizes pyproject.toml and poetry.lock files for dependency management, akin to Npm for JavaScript/Node.js and Cargo for Rust.
- **Integration:** Compatible with pyenv/pyenv-win for Python interpreter management.
- **Challenges:** May present a steeper learning curve due to strict dependency management.


## 6. pip
- **Usage:** Recommended solely for installing poetry, akin to using Internet Explorer solely for downloading Chrome.

# Reference
[Zhihu](https://zhuanlan.zhihu.com/p/663735038)