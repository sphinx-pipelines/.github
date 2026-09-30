# Welcome to the Sphinx Pipeline Organization
This workspace serves as a live, interactive reference dedicated to modern Python repository hygiene, automated documentation workflows, and robust Sphinx compilation pipelines. Instead of treating documentation as a static afterthought, these sandboxes will demonstrate how to treat technical manuals as a core engineering component that's fully integrated in your project, automatically tested, and bulletproof.

## Example repositories
* **sphinx-duo-code**: This is a stand-alone source repository that's part of a decoupled duo-repository framework and that serves as the isolated target for its companion documentation-pipeline repository.
* **sphinx-duo-docs**: This is a stand-alone Sphinx repository that's part of a decoupled duo-repository framework that demonstrates cross-repository commits, absolute configurations, and external path-routing.
* **sphinx-mono**: This is a unified all-in-one repository framework that demonstrates atomic commits, relative configurations, and internal path-routing.

## Demonstrated features
* **Compatibility tests:** Local compatibility tests that use `tox` to ensure that your documentation passes the same checks used by the GitHub CI pipeline before pushing changes to the repository.
* **Continuous Integration workflows:** GitHub Actions configurations that compile docstrings and package distributions seamlessly on every commit.
* **Environmental verification guards:** Local bash-wrappers that validate the directory layout before triggering build systems.
* **Hyperlink linting:** Automated linting that dynamically hunts down and flags broken references or dead assets.
* **Simplified hyperlink auditing:** Unique configuration that simplifies the management of hyperlinks by allowing the use of plain-text URLs.

## Organization layout

```text
sphinx-pipeline/                      # The front door of this organization
├── .github/                          # Directory for GitHub
│   └── profile/                      # Directory for control of main organization page
│       └── README.md                 # Main document for the organization (you are here)
│
├── sphinx-duo-code/                  # Split repo - Component A (Python code)
│   ├── codebase/                     # Directory for code
│   |   └── example.py                # Python module with reST docstrings
|   ├── .gitignore                    # Defensive tracking shield (ignores build artifacts)
|   ├── LICENSE                       # License
|   └── README.md                     # Main document for the repository
│
├── sphinx-duo-docs/                  # Split Repo - Component B (Sphinx pipeline)
│   ├── .github/                      # Directory for GitHub
│   │   └── workflows/                # Directory for GitHub workflows
│   │       └── ci.yml                # Advanced split-path CI pipeline
│   ├── sphinx/                       # Directory for Sphinx
│   │   ├── resources/                # Directory for engine assets and data drawers
│   │   │   ├── images/               # Directory for images and visual assets
│   │   │   ├── rst/                  # Directory for all other reST files
│   │   │   │   ├── installation.rst  # Documentation
│   │   │   │   └── usage.rst         # Documentation
│   │   │   ├── scripts/              # Directory for scripts (build, cleanup, linting, or automation)
│   │   │   ├── static/               # Directory for custom CSS or fonts        
│   │   │   └── templates/            # Directory for custom HTML structural layouts
│   │   ├── conf.py                   # Sphinx configuration matrix
│   │   └── index.rst                 # Sphinx documentation master layout file (entry-page/gatekeeper)
|   ├── .gitignore                    # Defensive tracking shield (ignores build artifacts).
|   ├── LICENSE                       # License
|   └── README.md                     # Main document for the repository
│
└── sphinx-mono/                      # Combined repository (unified monorepo).
    ├── .github/                      # Directory for GitHub
    │   └── workflows/                # Directory for GitHub workflows
    │       └── ci.yml                # Flat internal CI pipeline
    ├── codebase/                     # Directory for a demonstration code-base
    │   └── example.py                # Python module with reST docstrings
    ├── sphinx/                       # Directory for Sphinx
    │   ├── resources/                # Directory for engine assets and data drawers
    │   │   ├── images/               # Directory for images and visual assets
    │   │   ├── rst/                  # Directory for all other reST files
    │   │   │   ├── installation.rst  # Documentation
    │   │   │   └── usage.rst         # Documentation
    │   │   ├── scripts/              # Directory for scripts (build, cleanup, linting, or automation)
    │   │   ├── static/               # Directory for custom CSS or fonts        
    │   │   └── templates/            # Directory for custom HTML structural layouts
    │   ├── conf.py                   # Sphinx configuration matrix
    │   └── index.rst                 # Sphinx documentation master layout file (entry-page/gatekeeper)
    ├── .gitignore                    # Defensive tracking shield (ignores build artifacts)
    ├── LICENSE                       # License
    └── README.md                     # Main document for the repository
```

*Need an automated documentation-engine or pipeline tune-up for your project? Explore the examples, copy the scripts, or reach out to adapt these workflows to your code-base.*
