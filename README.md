# hello-astro
A TTS-flavored [Copier](https://copier.readthedocs.io/) template for creating and maintaining Astro applications

## Why this project

This template supports scaffolding and maintaining Astro-based federal applications, configured to the local tastes of TTS. 

It's suitable for standalone use or composition with [other `GSA-TTS/hello-*` templates](https://github.com/orgs/GSA-TTS/repositories?type=all&q=hello-).

## Features
- **Multiple Astro templates:**
  - astro-plain: Minimal Astro starter (default, for now)
  - [pages-site-gantry](https://github.com/cloud-gov/pages-site-gantry): Advanced starter CI/CD, styled with the USWDS, integrated with PayloadCMS

## Requirements
- [uv](https://docs.astral.sh/uv/getting-started/installation/) (for running Copier)
- [git](https://git-scm.com/)

## Usage
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

## Tasks
After copying, the following tasks are run automatically in the destination folder:
- `git init .`

Follow instructions in the README.md in the destination folder to work with the new site.

## Directory Structure
- `templates/astro-plain/`: Template for the minimal Astro starter
- `templates/pages-site-gantry/`: cg-pages' advanced starter with extra features, USWDS, etc.

## Contributing

See [CONTRIBUTING](CONTRIBUTING.md) for additional information.

## Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
