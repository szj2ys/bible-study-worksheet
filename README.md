# Bible Study Worksheet Maker

A small, offline-friendly worksheet for careful Bible reading. Fill in a passage, note its context, separate observations from interpretation, record questions and sources, and choose a practical response.

This is a working tool, not an AI answer generator. It was created by [TrustBible](https://trustbible.org/), which provides Bible reading and Scripture-referenced questions and answers. The worksheet runs independently of that service.

## Use it

1. Download `index.html` and open it in any current browser. No installation or account is needed.
2. Enter your passage and the Bible edition you use, then work through the four sections.
3. **Save worksheet file** downloads editable JSON. **Open saved file** restores it locally.
4. **Print worksheet** opens your browser's print dialog. Print to paper or save as PDF. Print the empty form for a blank study sheet.

The example is a set of study prompts, not a claimed interpretation of John 15.

## Privacy and limits

- No network requests, analytics, AI calls, external scripts, or server-side storage are used by the worksheet.
- Notes live in memory until you close or refresh the tab. Save a file if you want to keep them.
- A downloaded JSON file or PDF contains your notes. Keep it private when appropriate; take care on shared devices.
- No Bible text is bundled, so you can use your preferred translation and respect its quotation permissions.
- The worksheet does not establish the meaning of a passage or replace the Bible, pastoral guidance, or discussion with your community. Check claims and sources yourself.

The static hosting provider may keep ordinary access logs when you first load an online copy. Offline use of the downloaded HTML requires no connection.

## File format

Saved files contain `schema: "trustbible-study-worksheet-v1"` and a `fields` object with `title`, `date`, `passage`, `translation`, `context`, `observations`, `questions`, and `response`. Import checks the schema, field types, lengths, and date shape before replacing notes. Text is inserted as form values, never interpreted as HTML. Files larger than 100 KB are rejected.

## Development

There are no dependencies or build steps. Edit `index.html`; use a local static server if desired, or open the file directly. Use ordinary browser tools to inspect the form, import/export behavior, and print layout. The interface uses associated labels, keyboard-operable controls, a live status message, and responsive layouts.

## Sources for further reading

The tool supplies a note-taking structure and does not reproduce a third-party study curriculum. Read the passage in a named Bible edition and record any sources you consult. [TrustBible's Bible reader](https://trustbible.org/bible/) is one optional reading resource; using it is not required.

## License

Original code and documentation are MIT licensed. No third-party Bible translation is relicensed here.
