# mkdocs-obsidian-demo

## How to build
1. Install python UV
2. Install tox as a tool
```bash
uv tool install tox --with tox-uv # use uv to install
tox --version # validate you are using the installed tox
tox r -e py312 # will use uv
tox --runner virtualenv r -e py312 # will use virtualenv+pip
```
3. Run mkdocs serve to see the site locally
```bash
 uv tool run tox run -e mkdocs -- serve
```
4. Run mkdocs build to build the site
```bash
 uv tool run tox run -e mkdocs -- build
```