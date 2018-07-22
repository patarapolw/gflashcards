# gflashcards

Google sheets-based flashcard maker

# Usage

```python
>>> from gflashcards import Flashcard
>>> fc = Flashcards(spreadsheet_id, sheet_name, path_to_token, path_to_clientsecrets)
>>> card = fc.quiz(ham_regex, tags=[spam_regex, nam_regex])
>>> card
The front side of the card is shown on Jupyter Notebook. Images included. Both Markdown and HTML works.
>>> card.show()
The back side of the card is shown.
```

The `path_to_token` and `path_to_clientsecrets` can be omitted, and default to `user/token.json` and `user/credentials.json`, respectively.

`sheet_name` can be omitted and default to "flashcards".

`spreadsheet_id` can be extracted from the URL of the Google Sheets.

More information about `token`, `clientsecrets`, and `spreadsheet_id` can be viewed at https://developers.google.com/sheets/api/guides/concepts