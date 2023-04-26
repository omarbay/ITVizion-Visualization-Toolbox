# Installation

The backend of **ITV-visual** requires **Python 3.7** or later.

## Dependencies

See `requirements.txt` file for a list of
dependencies and versions. Additionally, you will need to install the `seeq` module with the appropriate version that
matches your Seeq server. For more information on the `seeq` module see [seeq at pypi](https://pypi.org/project/seeq/)

## User Installation Requirements (Seeq Data Lab)

If you want to install **ITV-visual** as a Seeq Add-on Tool, you will need:

- Seeq Data Lab (>= R52.1.5, >=R53.0.2, or >=R54)
- `seeq` module whose version matches the Seeq server version
- Seeq administrator access
- Enable Add-on Tools in the Seeq server

## User Installation (Seeq Data Lab)

The latest build of the project can be found [here](https://pypi.org/project/ITV-visual/) as a wheel file. The
file is published as a courtesy to the user, and it does not imply any obligation for support from the publisher.

1. Create a **new** Seeq Data Lab project and open the **Terminal** window
2. Run `pip install ITV_visual`
3. Import and use preferred classes in your python scripts by providing only the workbook url

or use directly as an add-on through the preferred seeq workbook.