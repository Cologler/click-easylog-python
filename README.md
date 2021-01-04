# click-easylog

A easy way to add log on click app.

## Usage

``` py
import click
from click_easylog import attach_logger_options, get_logger

@click.command()
@attach_logger_options()
def action()
    logger = get_logger()
```

`attach_logger_options` added some `loglevel` and `logto` options on the command:

- `logto` - `<stdout>`, `<stderr>` or any file name.
- `loglevel` - `info`, `warn`, etc.
