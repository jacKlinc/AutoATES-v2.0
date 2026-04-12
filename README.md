# AutoATES-v2.0
A fully automated algorithm used to provide ATES mapping for large areas.

## Setup (Ubuntu)

GDAL must be installed system-wide before installing the Python dependencies:

```bash
sudo apt-get install gdal-bin libgdal-dev
```

Install Python dependencies with [uv](https://docs.astral.sh/uv/):

```bash
uv python install 3.13
uv pip install setuptools numpy
uv sync --no-build-isolation
```

Verify the installation:

```bash
uv run python -c "from osgeo import gdal; print(gdal.__version__)"
```