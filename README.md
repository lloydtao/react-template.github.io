# vue-template.github.io

A GitHub Pages template to serve a Vue application.

## Getting Started

### Usage

Get started in minutes with these instructions:

1. Create a repository from this template.
2. Rename your repository to `<username>.github.io`.
3. Make sure that GitHub Pages uses the `build` branch. 

The branch can be selected at `Settings -> Options -> GitHub Pages -> Source`.

### Architecture

This is real simple:

- The `master` branch contains a Vue project.
- The `build` branch will contain the compiled Vue application.
- When you push to `master`, a GitHub Action compiles the updated project into `build`.

### Development

Any commits pushed or merged into `master` will trigger the build action.

These changes will be reflected on your GitHub Pages site after around 60 seconds.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
