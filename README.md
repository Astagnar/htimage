# htimage

This library has no dependencies in the form of other libraries. It works using only the built-in Python libraries and the browser installed on your system.

The following operating systems and browsers are currently supported:

| Browser | MacOS | Windows | Linux |
|---------|-------|---------|-------|
| Chrome  | ✅     | ✅       | ✅     |

## Installation

### From GitHub

Run the following command:

```bash
pip install git+https://github.com/Astagnar/htimage.git
```

## Examples

Get an image from the file:

```Python
from htimage import Htimage, Browsers


def main() -> None:
    hti = Htimage()
    
    hti.from_file(
        "D:/example.html",
        "D:/image.png",
        (1920, 1080),
        Browsers.CHROME
    )

if __name__ == '__main__':
    main()
```

Get an image from the link:

```Python
from htimage import Htimage, Browsers


def main() -> None:
    hti = Htimage()
    
    hti.from_url(
        "https://github.com/Astagnar",
        "D:/image.png",
        (1920, 1080),
        Browsers.CHROME
    )

if __name__ == '__main__':
    main()
```