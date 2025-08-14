# Quiz: yt-dlp (Intermediate)

1) Which output template placeholder returns the video identifier used by most sites (e.g., the YouTube short id)?

- A. `%(title)s`
- B. `%(id)s`
- C. `%(uploader)s`
- D. `%(format)s`

2) Which flag tells yt-dlp to attempt to download all available subtitle tracks (human-created)?

- A. `--write-sub`
- B. `--write-auto-sub`
- C. `--all-subs`
- D. `--sub-langs`

3) A video shows a “sign in to confirm you’re not a bot” page. Which yt-dlp option is specifically intended to reuse your local browser cookies on a machine where your browser is available?

- A. `--cookies cookies.txt`
- B. `--cookies-from-browser`
- C. `--username/--password`
- D. `--no-check-certificate`

4) You want to extract audio and output an MP3 file in one command. Which combination is correct?

- A. `--extract-audio --audio-format mp3`
- B. `--audio-only --format mp3`
- C. `-x --recode-video mp3`
- D. `--postprocessor-args mp3`

5) To ensure yt-dlp does not re-download videos across multiple runs and instead skips IDs already processed, which option should you use?

- A. `--no-overwrites`
- B. `--download-archive <file>`
- C. `--skip-download`
- D. `--continue`


Answer key

1) B — `%(id)s` is the site-specific short identifier for the video.

2) C — `--all-subs` requests all available (manual) subtitle tracks.

3) B — `--cookies-from-browser` reads cookies from your local browser profile (works locally).

4) A — `--extract-audio` (or `-x`) plus `--audio-format mp3` is the standard way.

5) B — `--download-archive <file>` records downloaded IDs and prevents future re-downloads.
