# Track Files Analysis

This script analyzes the files used in a track for the game IndyCar Racing 2 (ICR2). It identifies all `.3do` and `.mip` files used by a specified track and provides details about each file.

## Requirements

- Python 3.x

## Usage

1. Ensure that your track files are fully unpacked within a folder named after the track inside the `ICR2\TRACKS` directory.

2. Place the `analyze_track_files.py` script in the `ICR2\TRACKS` directory.

3. Open a command prompt and navigate to the `ICR2\TRACKS` directory:
    ```bash
    cd path\to\ICR2\TRACKS
    ```

4. Run the script with the track name as an argument:
    ```bash
    python analyze_track_files.py <trackname>
    ```

    Replace `<trackname>` with the name of your track (e.g., `detroi91`).

## Output

The script generates a file named `<trackname>_file_analysis.txt` containing:

- A list of all `.3do` files used by the track.
- Details of each `.3do` file, including file size.
- A list of all unique `.mip` files used by the track.
- Details of each `.mip` file, including width, height, and file size.
- A list of unused `.mip` files in the track folder.
- Totals for the number of `.mip` files, the total size of `.3do` files, the total size of `.mip` files, and the number of unused `.mip` files.

## Example

To analyze the `detroi91` track, run:
```bash
python analyze_track_files.py detroi91
