# hello-astro
A TTS-flavored [Copier](https://copier.readthedocs.io/) template for creating and maintaining Astro applications

## Why this project

This template supports scaffolding and maintaining Astro-based federal applications, configured to the local tastes of TTS. 

It's suitable for standalone use or composition with [other `GSA-TTS/hello-*` templates](https://github.com/orgs/GSA-TTS/repositories?type=all&q=hello-).

## Features
- **Multiple Astro templates:**
  - astro-plain: Minimal Astro starter
  - astro-uswds: Styled with the U.S. Web Design System v3.0 ([USWDS](https://designsystem.digital.gov/)), amenable to the [21st Century IDEA Act](https://digital.gov/resources/delivering-digital-first-public-experience#what-does-it-mean-to-modernize-websites) requirements

## Requirements
- [uv](https://docs.astral.sh/uv/getting-started/installation/) (for running Copier)
- [git](https://git-scm.com/)

## Usage

### Creating an application
1. [Install uv](https://docs.astral.sh/uv/getting-started/installation/) (if you haven't already)
2. Generate a new project...\
  ...from your local clone of the repository:
   ```sh
   uvx copier copy --trust ./hello-astro <destination-folder>
   ```
   ...or directly from the repository on GitHub:
   ```sh
   uvx copier copy --trust gh:GSA-TTS/hello-astro <destination-folder>
   ```
3. Answer the prompts:
   - Select which Astro template to use (`astro-plain` or `pages-site-gantry`).

### Updating the application later

If you'd like to...

- change your answers or 
- incorporate improvements made after you copied this template

...you can run the Copier `update` command: 

1. Make sure that your destination folder contains no uncommitted changes 
2. Update your destination folder from the most recently-tagged version of the template:
    ```
    uvx copier update --trust -a .hello-astro-answers.yml
    ```
   If necessary, you can specify a specific tag or gitref:
    ```
    uvx copier update --trust -a .hello-astro-answers.yml -r GITREF
    ```

To learn how updating works and what additional options are available, read [the Copier `update` documentation](https://copier.readthedocs.io/en/stable/updating/) .

Follow instructions in the README.md in the destination folder to work with the new site.

## Directory Structure
- `templates/astro-plain/`: Template for the minimal Astro starter
- `templates/astro-uswds/`: Minimal template styles with USWDS and oriented toward 21st Century IDEA requirements
- `templates/pages-site-gantry/`: cg-pages' advanced starter with extra features, USWDS, etc.

## Developing

To ensure that copies reflect your local changes to the template, specify the HEAD revision on the command-line. For example...

When copying:
```
uvx copier copy --trust -r HEAD <template-folder> <destination-folder>
```

When recopying:

```
uvx copier recopy --trust -r HEAD <destination-folder>
```

When updating: 

```
uvx copier update --trust -r HEAD <destination-folder>
```

There's [more information about this](https://copier.readthedocs.io/en/stable/faq/#while-developing-why-the-template-doesnt-include-dirty-changes) in the Copier docs.

## Contributing

See [CONTRIBUTING](CONTRIBUTING.md) for additional information.

## Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
