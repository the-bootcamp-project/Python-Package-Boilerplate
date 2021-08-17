# Files that need change if clone a Repo

- [ ] Change ENV PYTHONPATH in Dockerfile
- [ ] Change banditArgs -r path
- [ ] Change Package Source Folder in ./lib
- [ ] Change Package name in makefile
- [ ] Update README.md
  - [ ] Change Headine to Gitlab Project Title
  - [ ] Change Badge URL
  - [ ] Change Installation section
  - [ ] Change Usage section
  - [ ] Change Roadmap section
  - [ ] Change Acknowledgements section

1. Dockerfile in `.devcontainer`

```bash
ENV PYTHONPATH "${PYTHONPATH}:/workspaces/WORKSPACE_DIRECTORY/"
```

2. **setting.json** in **`.vscode`**

```json
"python.linting.banditArgs": [
    "-c bandit.yml",
    "-r lib/PACKAGE_NAME"
],
```

3. Package subfolder in **`./lib`**

```bash
lib\PACKAGE_NAME
```

4. Package name in **makefile**

```bash
package=PACKAGE_NAME
```

5. Headline in **README.md**

```html
<h1 align="center">Project Title from Gitlab Repository</h1>
```

6. Package name and Project Title in **Badges** Source

```html
<div align="center">
![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg?style=for-the-badge)
![PyPI](https://img.shields.io/pypi/v/PACKAGE_NAME?style=for-the-badge)
![PyPI - Status](https://img.shields.io/pypi/status/PACKAGE_NAME?style=for-the-badge)
![PyPI - Implementation](https://img.shields.io/pypi/implementation/PACKAGE_NAME?style=for-the-badge)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PACKAGE_NAME?style=for-the-badge)
![PyPI - Wheel](https://img.shields.io/pypi/wheel/PACKAGE_NAME?style=for-the-badge)
![PyPI - License](https://img.shields.io/pypi/l/PACKAGE_NAME?style=for-the-badge)

![Bootcamp Project: Project Title from Gitlab Repository](https://img.shields.io/badge/Bootcamp-Project-blue?style=for-the-badge)
</div>
```

7. **Installation** section in README.md

```bash
pip install --user *PACKAGE_NAME*
```

8. Documention Link in **Usage** section

`_For more examples, please refer to the [Documentation](https://PACKAGE_NAME.rtfm.page)_`

9. Repository Issue Link in **Roadmap** section

`See the [open issues](PACKAGE_GITLAB_URL/-/issues) for a list of proposed features (and known issues).`

10. Project Title in **Acknowledgements**

`Thanks for these awesome resources that were used during the development of the **Project Title from Gitlab Repository**:`
