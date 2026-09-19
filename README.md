# Hot Wheels Vault v6 — Camera Fixed

v6 specifically fixes the mobile photo-selection problem seen on Samsung Internet.

Changes:
- Separate **Take Photo** and **Gallery** buttons.
- Uses explicit button -> file input activation rather than relying on a styled label.
- Does not use `display:none` for the file input.
- Handles both `change` and the selected File object explicitly.
- Uses FileReader/DataURL for the preview and OCR pipeline instead of relying on a `content://`/blob URL.
- The catalog/OCR workflow from v5 remains.

If Camera does not work in a particular browser, Gallery should still let you select the photo and continue scanning.
