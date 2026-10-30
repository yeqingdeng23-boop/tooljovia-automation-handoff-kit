# A small-team client handover checklist for photo reports and subtitles

By the ToolJovia team

I help build ToolJovia. When a job includes both a photo issue report and a captioned video, the files may come from separate workflows. This checklist helps a small team assemble a clear handover. Use only the sections that fit the agreed work; neither tool sends files or manages the handover for you.

## 1. Agree what the client should receive

- [ ] Name the project, the intended recipient and the agreed delivery date.
- [ ] List each promised file and its purpose: a readable report, an editable issue list, or a subtitle file for a particular video or player.
- [ ] Identify who will check each file and who will deliver it. Record open questions instead of guessing what the client expects.
- [ ] Agree a suitable, authorized delivery method and check the recipient can open the chosen formats.

## 2. Prepare the photo issue report

Use the free [Photo Issue Report Builder](https://tooljovia.com/tools/photo-issue-report-builder/) for up to 10 issues. Each can include a location, description, status, assignee and one optional JPEG or PNG. Project name and issue descriptions are required for PDF and CSV.

- [ ] Match each photo to the right issue and location. Describe observations and proposed next steps separately in the description; do not present an unverified diagnosis as fact.
- [ ] Review photos and text for addresses, names, people or other details the recipient should not receive; remove unnecessary material before delivery.
- [ ] Download the PDF for reading and, if useful, the CSV issue list. Save JSON if someone needs a restorable editable copy.
- [ ] Open the actual downloaded files and check them. PDF uses a limited Latin font; unsupported characters can prevent PDF export. Separate CSV and JSON downloads preserve UTF-8.

The report is processed in the browser without an account. It does not autosave: save the JSON before closing if you need to restore the draft. Only include editable files and photos in the handover when the client is meant to receive them.

## 3. Prepare the subtitles, when included

Keep the original caption file. The free [Plain Subtitle Workbench](https://tooljovia.com/tools/subtitle-workbench/) processes pasted text in your browser without an account.

- [ ] Confirm the required format and the exact video version with the recipient.
- [ ] If a timing shift is needed, choose its direction deliberately: **+125 ms** moves cues later; **-125 ms** moves them earlier. Apply only the shift your review calls for.
- [ ] Save the output, read it and test it against the intended video in the intended player or course platform. The workbench does not play the video or automatically repair overlaps.
- [ ] Check whether the source uses timing settings or WebVTT NOTE, STYLE, REGION or header metadata. These are outside the workbench's plain-cue profile, so use another suitable workflow when they must be preserved.

## 4. Assemble and review the handover

- [ ] Put only the agreed deliverables in a clearly named folder. Keep a separate working backup of originals and the JSON if appropriate.
- [ ] Add a short handover note listing filenames, what each contains, the video version used for caption testing, and any unresolved issues or checks still pending. Do not mark an unperformed check as passed.
- [ ] Reopen the files from the folder intended for delivery. Check the PDF pages, CSV columns and subtitle text; verify the captions against the intended player if that was part of the work.
- [ ] Use the agreed delivery method. Tell the recipient what feedback or decision is needed and who will handle it; separately confirm receipt through your normal process.

The tools create files from the information you enter; they do not verify a repair, establish client approval, provide shared team storage or send the handover.
