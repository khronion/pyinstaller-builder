# pyInstaller-Builder

pyInstaller-Builder is a Github Actions workflow that compiles a Python script into Windows, Linux, and macOS.

## Installation

Copy [`.github/workflows/build-release.yml`](https://github.com/khronion/pyinstaller-builder/blob/main/.github/workflows/build-release.yml) into your repository and edit the environment variables to match your repository:

- `APP_NAME`: Name of the Python script to be compiled
- `PKG_NAME`: Name for the packaged executable file

Next, ensure that `requirements.txt` is created and contains all of your project's dependencies (even if it is empty). The workflow will fail if this file is not present!

## Usage

The workflow will automatically run upon the creation of a tagged release and generate builds for Windows AMD64, Linux AMD64, and macOS Intel. For an demonstration, [see this repository's releases](https://github.com/khronion/pyinstaller-builder/releases).

## License
[GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
