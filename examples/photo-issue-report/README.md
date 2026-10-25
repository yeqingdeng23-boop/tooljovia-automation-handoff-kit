# Photo issue report demo

Three made-up issues and diagrams show how the same records appear in a report, a checklist and an editable backup. This is a synthetic demonstration, not a client inspection.

[Open the free Photo Issue Report Builder](https://tooljovia.com/tools/photo-issue-report-builder/)

## Look at the deliverables

| File | What to do with it |
|---|---|
| [Sample PDF](sample.pdf) | Read the illustrated report. |
| [Sample CSV](sample.csv) | Compare issue IDs, locations, descriptions, owners and statuses with the PDF. |
| [Editable JSON draft](sample.json) | Download it, then import it into the web tool to restore the same three records and images. |

Use GitHub's **Download raw file** control to save the JSON itself before importing it.

## Try the same task

1. Open the web tool and choose **Load synthetic example**. No file download is needed to start.
2. Review the three synthetic issues, then change a description, assignee or status while keeping its ID.
3. Choose **Save PDF report** and **Save matching CSV**. Compare the issue IDs and order in both files.
4. Use **Save JSON backup** if you want to resume editing later.

To keep the current report version, save a JSON backup before adding an optional arrow. Choose **Add an arrow**, set its two endpoints, then choose **Apply arrow** or **Cancel**. Applying flattens one red arrow into the report JPEG used in the PDF and JSON backup. It cannot be removed separately after restore; your original image file is unchanged.

For a property or construction handoff, the [photo punch list guide](https://tooljovia.com/photo-punch-list/) shows how to write clear issue notes, check the same IDs in the PDF and CSV, and continue editing from a saved JSON draft.

The builder handles up to 10 items. Processing stays in your browser; the tool does not upload your images or report contents. PDF text uses a limited Latin character set. Unsupported characters stop PDF export with an error; CSV and JSON preserve the UTF-8 text.

## Tell us what you need

Have a current reporting task? [Open an email draft](mailto:yeqingdeng23@gmail.com?subject=ToolJovia%20photo%20report%20feedback) and describe what you need to deliver, what you use now and the one output you are missing. Sending is optional and manual. Please leave out private photos, client information and credentials.

These sample files are a separate optional download. The automation handoff ZIP linked from the repository root contains its original 19 files.
