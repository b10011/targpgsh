# targpgsh

Simple self-extracting encrypted and optionally compressed tar archives. The goal is to have a very portable and easy to use format.

This script is not intented to be the most beautiful and most tought-out piece of code. It will likely continue to be a hacky solution forever.

## Usage

```
Usage: targpgsh [--gzip|--xz|--raw] OUTPUT_PATH DATA_FILES...
```

## Example

```bash
# Create output.sh archive
targpgsh --gzip output.sh file1.txt file2.txt file3.txt

# Extract the contents to ./output_subdirectory
bash output.sh -d ./output_subdirectory
```
