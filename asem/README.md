# Flow to Download Audio Files Using yt-dlp

This flow automates the process of downloading audio from YouTube using **yt-dlp**.  
It scans a FileFlows library for **TXT** or **CSV** files containing lists of URLs and executes yt-dlp for each entry.

The resulting audio files are saved as **MP3s** in a folder created next to the source list file.  
That folder is named after the value defined as **Album**.

---

## How It Works

- The flow looks for `.txt` or `.csv` files in the library.
- Each file is parsed for YouTube URLs.
- yt-dlp is executed for every URL found.
- Audio is extracted and converted to MP3.
- Output files are stored in an album-named directory beside the list file.

---

## Setup Instructions

1. Import the flow into **FileFlows**.
2. Create a new **Files** library.
3. Name the library.
4. Assign the imported flow to this library.
5. Restrict file extensions to: `.txt`, `.csv`

---

## Preparing URL Lists

- Create TXT or CSV files inside the library directory or any subfolder.
- Each file should contain a list of YouTube URLs (one per line).
- The filename **must include the word `list`**.

---

## Processing & Output

- On the next library scan, FileFlows will detect and process the list files.
- All listed items will be downloaded as **MP3 files**.
- A new folder will be created next to the list file:
  - Named after the **Album** value
  - Containing all downloaded audio files




