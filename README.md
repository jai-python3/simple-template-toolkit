# simple-template-toolkit

Simple templating for all your simple templating projects

- [simple-template-toolkit](#simple-template-toolkit)
  - [Improvements](#improvements)
  - [Use Cases](#use-cases)
  - [Class Diagrams](#class-diagrams)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Exported scripts](#exported-scripts)
  - [Contributing](#contributing)
  - [To-Do/Coming Next](#to-docoming-next)
  - [CHANGELOG](#changelog)
  - [License](#license)



## Improvements

Please see the [TODO](docs/TODO.md) for a list of upcoming improvements.


## Use Cases

<img src="use_cases.png" width="400" height="300" alt="Use Cases diagram">


## Class Diagrams

![class diagrams](class_diagrams.png)

## Installation

Please see the [INSTALL](docs/INSTALL.md) guide for instructions.

## Usage

Use Case 1:

```python
from simple_template_toolkit import STTManager

tm = STTManager()

tm.make_substitutions(
  template_file=template_file,  # the template file containing your placeholder values
  outfile=outfile, # the file that should be written out
  lookup=lookup # a dictionary contain placeholders for keys and corresponding values replace with
)
```

Use Case 2:

```python
from simple_template_toolkit import STTManager

tm = STTManager()

tm.inject_lines(
  template_file=template_file,  # the template file containing your placeholder values
  outfile=outfile, # the file that should be written out
  lookup=lookup 
)

# The lookup is a dictionary where the keys are
# are the line anchors where the lines of code should be inserted.
# The values are lists (arrays) containing the lines of code that
# should be inserted at that line anchor.
```

## Exported scripts

The following exported console script is available for use:

- make-substitutions
- insert-lines

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## To-Do/Coming Next

Please view the listing of planned improvements [here](docs/TODO.md).

## CHANGELOG

Please view the CHANGELOG [here](docs/CHANGELOG.md).

## License

[GNU AFFERO GENERAL PUBLIC LICENSE](docs/LICENSE)
