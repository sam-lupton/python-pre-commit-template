# python-pre-commit-template
A template with some key pre-commit settings

Some less strict ruff formatting:

[tool.ruff]
line-length = 120
target-version = "py312"
select = [
    "ALL", # include all the rules, including new ones
]
ignore = [
    #### modules
    "A002",
    "A003",
    "ANN", # flake8-annotations
    "COM", # flake8-commas
    "C90", # mccabe complexity
    "DJ",  # django
    "EXE", # flake8-executable
    "T10", # debugger
    "TID", # flake8-tidy-imports

    #### specific rules
    "D100",   # ignore missing docs
    "D101",
    "D102",
    "D103",
    "D104",
    "D105",
    "D106",
    "D107",
    "D200",
    "D203",
    "D205",
    "D212",
    "D400",
    "D401",
    "D415",
    "DTZ001",
    "DTZ005", # ignore timezone warnings
    "E402",   # false positives for local imports
    "E501",   # line too long
    "FBT001",
    "FBT002",
    "INP001",
    "N803",
    "N806",
    "NPY002",
    "PD901",
    "PGH004",
    "PLE1205",
    "PLR0913",
    "PTH123",
    "S113",
    "TRY003", # external messages in exceptions are too verbose
    "TD002",
    "TD003",
    "T201",
    "PGH003",
    "FIX002", # too verbose descriptions of todos
    "RUF012",
    "S101", # ignore use of assert in unit tests
]
