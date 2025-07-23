This script could be used for rescaling of data stored in zarr arrays using Dask for parallelization on a LSF cluster/local machine. 
#### How to run
1. open command line terminal
2. install poetry tool for dependency management and packaging: https://pypi.org/project/poetry/
3. switch to the recompress_zarr/src directory:
    ``cd PATH_TO_DIRECTORY/recompress_zarr/src``
4. install python dependencies:
    ``poetry install``
5. run script using cli:
    ``poetry run python src/normalize.py --src="PATH_TO_SOURCE_DIRECTORY/input_file.zarr" --dest="PATH_TO_DEST_DIRECTORY/output_file.zarr" --global_min=188 --global_max=214  --workers=400 --data_type=uint8'``
