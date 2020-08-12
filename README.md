# vue-template.github.io

A GitHub Pages template to serve a Vue application.

## Getting Started

### Usage

Get started in minutes with these instructions:

1. Create a repository from this template (include all branches).
2. Rename your repository to `<username>.github.io`.
3. Make sure that GitHub Pages uses the `build` branch. 

The branch can be selected at `Settings -> Options -> GitHub Pages -> Source`.

*This may take a minute or two to update*.

### Architecture

This is real simple:

- The `master` branch contains a Vue project.
- The `build` branch will contain the compiled Vue application.
- When you push to `master`, a GitHub Action compiles the updated project into `build`.

### Development

Any commits pushed or merged into `master` will trigger the build action.

These changes will be reflected on your GitHub Pages site after around 60 seconds.

### Domain Names

**Apex Domain**

First, set your domain name within the GitHub repositry.

- In the `CNAME` file, replace `example.com` with your domain.

Second, configure your DNS host records with your domain provider.

- Create an **A** record for host "@" pointing to `185.199.108.153`.
- Create an **A** record for host "@" pointing to `185.199.109.153`.
- Create an **A** record for host "@" pointing to `185.199.110.153`.
- Create an **A** record for host "@" pointing to `185.199.111.153`.

**Subdomains**

You can configure a subdomain, such as `www.[example.com]`, in your DNS host records.

- Create a **CNAME** record for host "www" pointing to `<username>.github.io`.

### Infinite Hosting

Want to know what makes this awesome? You can have a repository for each and every subdomain.

1. Create a repository from this template with any name (include all branches).
2. Enable GitHub Pages for it (`Settings -> Options -> GitHub Pages -> Source`).
3. In the `CNAME` file, replace `example.com` with your apex and subdomain (i.e. `blog.[example.com]`).
4. With your domain provider, create a **CNAME** record for host "`[blog]`" pointing to `<username>.github.io`.

Why does this work? 

The repo's GitHub Pages already hosts itself at <username>.github.io/<repo>, since GitHub sets up the environment and deployment for you when you enable Pages.

The CNAME just puts it on its own subdomain, instead of in its own subdirectory.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
