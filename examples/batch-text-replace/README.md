# Replace the same text in two files

Try a fictional worked example before choosing files from your own work. The two inputs contain no client data.

## Try it

1. Download [inputs.zip](inputs.zip) and unzip it. It contains `old-a.txt` and `old-note.txt`. Do not select the ZIP itself in the tool.
2. Open the free [Batch Text File Replacer](https://tooljovia.com/tools/batch-text-file-replacer/).
3. Select both extracted `.txt` files. Enter `ACME` in **Find this exact literal** and `NOVA` in **Replace with this literal**. Match the capital letters exactly.
4. Choose **Run tool**. Check that the result shows **2 selected files**, **1 changed file** and **2 literal matches**. Choose **Download** to save `rewritten-text-files.zip`.
5. Unzip your result. Compare its separate files with the saved [sample-result.zip](sample-result.zip), which was previously exported from these fictional inputs.

If GitHub opens a ZIP file view, use **Download raw file** to save it.

## What to expect

| File | Result |
|---|---|
| `files/old-a.txt` | `Project NOVA / NOVA.` followed by its original LF line ending. Both occurrences change. |
| `files/old-note.txt` | `No matching client.` followed by its original CRLF line ending. The entire file stays unchanged. |
| `rewrite-evidence.json` | Each file's match count, byte sizes, SHA-256 values and exact source/output match positions. |

The two text files total **42 bytes before and after** replacement. The ZIP is larger because it also includes the report and archive structure. Compare the extracted text and counts; a later tool version may change report wording or ZIP metadata.

## Before using your own files

Processing runs locally in your browser. Original files are not overwritten; review the exported copies before using them.

The tool accepts 1–20 flat UTF-8 files, up to 1 MiB each and 2 MiB combined. It performs one case-sensitive literal replacement, with no regex, folder traversal or encoding guessing. Replacing text is not a syntax or meaning check.

These sample files are fictional practice material, separate from the version 0.3 worksheet ZIP. They are not client work or evidence of paid use.
