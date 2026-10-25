# Images to PDF: synthetic two-page demo

Try a two-page document handoff using made-up records. **TJ-DEMO-01** is a synthetic demonstration, not a customer job or a record of completed field work.

The four files in this example are:

- [Delivery checklist input](delivery-checklist.png) - first page, 1600 x 1200 PNG.
- [Field notes input](field-notes-issue-summary.png) - second page, 1600 x 1200 PNG.
- [Actual two-page PDF result](images.pdf) - downloaded from the website after preparing and adopting both pages.
- `README.md` - these instructions.

## Try it

1. Open [ToolJovia Images to PDF](https://tooljovia.com/tools/images-to-pdf/) and choose **Load example** to load both synthetic pages in order. You can also download the two PNGs above and select **both together** in the Images file picker. The tool accepts PNG, JPEG and WebP images; it does not accept SVG inputs.
2. For a quick two-page PDF, leave optional preparation off, select **Run tool**, then **Download**. A successfully loaded example uses A4, Portrait and 20-point margins. To reproduce the prepared PDF in this folder instead, continue with steps 3–6.
3. Enable **Prepare image pages before making the PDF (optional)**. Confirm that the checklist is first and field notes second; use **Move page up/down** if needed. Select each page and drag the four handles to the document corners. You can also focus a handle and use the arrow keys to adjust it. To reproduce the sample PDF using the listed corners, optionally enter the working-image coordinates in the table below. For your own images, choose corners for that document instead.
4. Keep the default **Color** mode, select **Preview preparation**, and compare the original and prepared page. Then explicitly select **Adopt preview for this PDF page**. Repeat for the other page. Previewing alone does not change the PDF.
5. Set **PDF page size** to **Image pixels as points**, **Page orientation** to **Portrait**, and **Margin points** to **0**. Select **Run tool**, then **Download**.
6. Open the PDF. Check that the checklist is first and field notes second, with the same project and item labels on both pages. Restore the original page or reset the tool if you want to start again. You can also leave preparation off for direct conversion.

For these two supplied PNGs, the preparation working image is **1154 x 866**. The prepared sizes below describe the saved example made with these exact coordinates. Choosing different corners can produce different dimensions. Coordinates are ordered top left, top right, bottom right, bottom left:

| Page | Four working-image corners | Prepared image and PDF page size |
| --- | --- | --- |
| Checklist | (180,115), (915,78), (942,736), (207,773) | 737 x 660 pixels; 737 x 660 PDF points |
| Field notes | (216,69), (951,102), (928,760), (193,726) | 737 x 659 pixels; 737 x 659 PDF points |

## What to check

Both pages show **SYNTHETIC DEMO** and **Project TJ-DEMO-01**. The checklist has **ITEM-01: READY**, **ITEM-02: REVIEW**, and **ITEM-03: PENDING**. The notes repeat those states and say that approval has not been recorded. These are fictional labels, not real approvals.

The image conversion runs locally in your browser. Preparation can reduce resolution; Color is the default. Black and white is optional and can thicken small text or add speckle. No OCR or searchable text layer is added.

For larger sets, such as 20 job photos and three receipt images, optional batch preparation scales images down using the currently adopted crop or black-and-white version, or the original when no preparation has been adopted. Review each proposed page and check receipt text, then explicitly adopt the batch once; individual preview-and-adopt steps are not required for every page. Originals remain available; restoring a page returns to its original image, not an earlier crop. Choose **Run tool**, then **Download**, to get the PDF. Batch preparation does not raise input, pixel or output limits and may not make every set fit. It runs in your browser without uploading files or requiring an account or email address.

To combine job photos, receipt images and a supported existing PDF, create the image pages with [Images to PDF](https://tooljovia.com/tools/images-to-pdf/), then open [PDF Page Organizer](https://tooljovia.com/tools/pdf-page-organizer/).
For a two-page image PDF selected as file 1 and another compatible PDF as file 2, use `1:1-2,2:1`; file numbers follow the actual selected-file order.
The Organizer accepts up to 10 PDFs, 20 MiB each, 50 MiB together, 200 pages per input and 200 selected output pages; separate image and pixel limits still apply, and digitally signed PDFs are rejected.
Follow the [mixed-file handoff steps](https://tooljovia.com/tools/images-to-pdf/#images-pdf-job-handoff) for compatibility limits, then check the final page order and receipt readability before sharing.

## Optional task feedback

[Share a current task or missing deliverable](https://github.com/yeqingdeng23-boop/tooljovia-automation-handoff-kit/issues/new?template=current-task.yml). Feedback is voluntary. GitHub issues are public and require GitHub sign-in; do not attach private documents, photos, personal details or credentials.

No paid service is currently offered.
