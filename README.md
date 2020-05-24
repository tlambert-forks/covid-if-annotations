# napari-covid-if-annotations

[![License](https://img.shields.io/pypi/l/napari-covid-if-annotations.svg?color=green)](https://github.com/napari/napari-covid-if-annotations/raw/master/LICENSE)
[![PyPI](https://img.shields.io/pypi/v/napari-covid-if-annotations.svg?color=green)](https://pypi.org/project/napari-covid-if-annotations)
[![Python Version](https://img.shields.io/pypi/pyversions/napari-covid-if-annotations.svg?color=green)](https://python.org)
[![tests](https://github.com/constantinpape/napari-covid-if-annotations/workflows/tests/badge.svg)](https://github.com/constantinpape/napari-covid-if-annotations/actions)
[![codecov](https://codecov.io/gh/constantinpape/napari-covid-if-annotations/branch/master/graph/badge.svg)](https://codecov.io/gh/constantinpape/napari-covid-if-annotations)

Annotation Tool for immunofluorescence assay images

----------------------------------

## Usage

After installing the plugin, you can run
```
python launch.py
```
to launch the annotation tool. You can then drag and drop data to annotate onto the viewer.
Or you can start the tool with data already via:
```
python launch.py --path /path/to/data.h5
```

Example data is [available here](https://oc.embl.de/index.php/s/IghxebboVxgpraU).

Keybindings:
- `u` update point and edge layer from the segmentation corrections and semantic annotations.
- `h` toggle visibility of already annotated segments.
- `.` cycle through the annotations for a selected point
- `t` toggle annotation cycling by mouse click (not working yet!)


## Installation

### From source

Set up a conda env with all dependencies:

```
conda create -c conda-forge -n test-annotations napari scikit-image h5py pandas
```
Then install the napari plugin (in dev mode) via
```
pip install -e .
```

## Acknowledgements

This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.

<!--
Don't miss the full getting started guide to set up your new package:
https://github.com/napari/cookiecutter-napari-plugin#getting-started

and review the napari docs for plugin developers:
https://napari.org/docs/plugins/index.html
-->

## Contributing

Contributions are very welcome. Tests can be run with [tox], please ensure
the coverage at least stays the same before you submit a pull request.

## License

Distributed under the terms of the [MIT] license,
"napari-covid-if-annotations" is free and open source software

## Issues

If you encounter any problems, please [file an issue] along with a detailed description.

[napari]: https://github.com/napari/napari
[Cookiecutter]: https://github.com/audreyr/cookiecutter
[@napari]: https://github.com/napari
[MIT]: http://opensource.org/licenses/MIT
[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
[file an issue]: https://github.com/constantinpape/napari-covid-if-annotations/issues
[napari]: https://github.com/napari/napari
[tox]: https://tox.readthedocs.io/en/latest/
[pip]: https://pypi.org/project/pip/
[PyPI]: https://pypi.org/
