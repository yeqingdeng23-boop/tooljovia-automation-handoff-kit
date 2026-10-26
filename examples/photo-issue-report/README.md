# Photo issue report demo

Three made-up issues and diagrams show how the same records appear in a report, a checklist and an editable backup. This is a synthetic demonstration, not a client inspection.

[Open the free Photo Issue Report Builder](https://tooljovia.com/tools/photo-issue-report-builder/)

## Look at the deliverables

| File | What to do with it |
|---|---|
| [Sample PDF](sample.pdf) | Read the illustrated report. |
| [Sample CSV](sample.csv) | Compare issue IDs, locations, descriptions, owners and statuses with the PDF. |
| [Editable JSON draft](sample.json) | Download it, then import it into the web tool to restore the same three records and images. |

[Download the prepared synthetic sample ZIP](https://raw.githubusercontent.com/yeqingdeng23-boop/tooljovia-automation-handoff-kit/main/examples/photo-issue-report/sample-handoff.zip). It contains the PDF, CSV and editable JSON with embedded synthetic report images. Review before sharing.

Use GitHub's **Download raw file** control to save the JSON itself before importing it.

## Try the same task

1. Open the web tool and choose **Load synthetic example**. No file download is needed to start.
2. Review the three synthetic issues, then change a description, assignee or status while keeping its ID.
3. Choose **Download handoff ZIP** to save the PDF report, matching CSV checklist and editable JSON from one report snapshot. The JSON includes report photos, so review the contents before sharing. You can still save PDF and CSV separately. Compare the issue IDs and order in the PDF and CSV.
4. To continue editing from a ZIP, unzip it first, choose **Restore JSON backup** and select the extracted `.json` file, not the ZIP. Use **Save JSON backup** separately to keep an unfinished draft, including an empty project name or description.

To start with your own JPEG or PNG files, choose **Add photos as draft issues**. Each photo becomes one draft issue; the report can contain up to 10 issues in total. The whole batch is added only after every photo passes processing. Review the order, then add your project name and a description for each new issue before saving a PDF or CSV. Save JSON to keep an unfinished draft.

To keep the current report version, save a JSON backup before adding an optional arrow. Choose **Add an arrow**, set its two endpoints, then choose **Apply arrow** or **Cancel**. Applying flattens one red arrow into the report JPEG used in the PDF and JSON backup. It cannot be removed separately after restore; your original image file is unchanged. You can use **Undo last arrow** once for the most recently applied arrow in the current tab. This restores just that photo and keeps later text, IDs and order edits. Applying another arrow replaces this temporary undo; it is not included in JSON backups.

For a property or construction handoff, the [photo punch list guide](https://tooljovia.com/photo-punch-list/) shows how to write clear issue notes, check the same IDs in the PDF and CSV, and continue editing from a saved JSON draft.

The builder handles up to 10 items. Processing stays in your browser; the tool does not upload your images or report contents. PDF text uses a limited Latin character set. Unsupported characters stop PDF and handoff ZIP export with an error; the separate CSV and JSON exports preserve UTF-8 text.

## Tell us what you need

Have a current reporting task? [Open an email draft](mailto:yeqingdeng23@gmail.com?subject=ToolJovia%20photo%20report%20feedback) and describe what you need to deliver, what you use now and the one output you are missing. Sending is optional and manual. Please leave out private photos, client information and credentials.

Prefer a public GitHub reply? [Share a current task in an Issue](https://github.com/yeqingdeng23-boop/tooljovia-automation-handoff-kit/issues/new?template=current-task.yml). An Issue is public and requires a GitHub account; share a general task description only.

These sample files are a separate optional download. The worksheet ZIP linked from the repository root contains 19 editable files.
