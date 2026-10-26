# Two-cue subtitle handoff: SRT to WebVTT

Give a website or video editor a small subtitle pair with an explicit timing change. These original, fictional files are separate from the 19-file version 0.2 handoff ZIP.

- [SRT input](two-cues-original.srt)
- [WebVTT result, shifted 125 ms later](two-cues-shifted-125ms.vtt)

Open each file as UTF-8 text, or use GitHub's **Raw** view to save it. The SRT uses comma milliseconds. The WebVTT adds a `WEBVTT` header and uses decimal points. Cue IDs 7 and 11 and their text are retained.

| Cue | Original start–end | Shifted start–end | Duration, unchanged |
|---|---|---|---|
| 7 | 0.500–1.750 s | 0.625–1.875 s | 1.250 s |
| 11 | 2.250–4.000 s | 2.375–4.125 s | 1.750 s |

Both ends move later by 125 ms; this is a demonstration offset, not a timing recommendation. The text deliberately includes `café` (U+00E9), `café` (U+0065 U+0301) and 🧰✅. The two accented forms remain distinct sequences.

## Try the same conversion

1. Open the free [Subtitle Workbench](https://tooljovia.com/tools/subtitle-workbench/) and paste the complete SRT into Input.
2. Choose SRT input, WebVTT output and a 125 ms shift. Run the tool, review the text and download the result. Load example remains available for the tool's default starter.
3. Tell your recipient which format and offset you are handing over. Check the file in the intended editor or player before using it with real media.

No media is included. This plain two-cue pair does not establish playback synchronisation or compatibility with every player. Conversion runs in your browser without requiring an account or email address.
