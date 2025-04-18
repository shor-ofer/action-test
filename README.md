# HelloWorld C++ Project

This project demonstrates a simple "Hello, World!" C++ application built using CMake. The project is set up with GitHub Actions to automatically build and release executables for Windows, Linux, and macOS platforms upon creating a new tag.

## Build Process

- **CMake** is used to configure and build the project.
- **GitHub Actions** automates the build process across multiple platforms.
- Upon tagging a release (e.g., `v1.0.0`), the corresponding executables are built and uploaded as zip files to the GitHub Release.

## Creating a Release

To create a new release:

1. Commit your changes.
2. Tag the commit with a version number, e.g., `git tag v1.0.0`.
3. Push the tag to GitHub: `git push origin v1.0.0`.

GitHub Actions will automatically build the project for all specified platforms and upload the executables as release assets.

## License

This project is licensed under the MIT License.
