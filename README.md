# FDG 2023 Website

## How to update the main website

The main website at <http://www.fdg2023.org/> is automatically updated when
pushing to the `main` branch of this repository.

## How to generate the website locally

To generate the website locally, [Git](https://git-scm.com/) and
[Python](https://www.python.org/) are hard requirements.

To generate the website for the first time in any given computer, the following
commands should be executed in the console:

```
git clone https://github.com/VideojogosLusofona/fdg_2023_website.git
cd fdg_2023_website
python -m venv env
source ./env/bin/activate
pip install --upgrade pip
pip install mkdocs-material mkdocs-macros-plugin
mkdocs serve
```

The site can be visualized locally by following the link provided by the last
command.

The following times, site generation requires fewer commands:

```
cd fdg_2023_website
source ./env/bin/activate
mkdocs serve
```

On Windows the `source ./env/bin/activate` command should be replaced with
`env\Scripts\Activate.ps1` or `env\Scripts\activate.bat` (for PowerShell or
cmd.exe consoles, respectively).

## Editing and configuring the website

* The website is configured by modifying the [`mkdocs.yml`](mkdocs.yml) file.
* Website contents can be changed and updated by editing the contents of the
  [`docs`](docs/) folder.
* The system used to generate this website is
  [MKDocs Material](https://squidfunk.github.io/mkdocs-material/).
