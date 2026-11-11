# Privacy and local storage

Folder Reader reads files you choose and saves reading progress locally.

- No backend, sign-in, analytics, or document uploads.
- Source documents stay in place and are not edited by Folder Reader.
- History lives at `~/Library/Application Support/FolderReader/history.json`.
- History contains local paths, file sizes and modification dates, viewed/reviewed state, PDF page numbers, recent folders, and security-scoped folder bookmarks. It does not copy document contents.
- Quick Look, PDFKit, and AVKit render previews. Opening an online-only cloud file may cause its storage provider to download it.
- “Open original” hands the file to its default application; that application's behavior is separate.
- The experimental app is currently unsandboxed. Production sandboxing is planned.
- Public GitHub issues are public: do not attach private documents or your history file.

There is no automatic update checker in v0.1.2.
