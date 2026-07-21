# telegram-cache-decryption

**Update**: Last tested to work with Telegram Desktop version: 7.0.2.

Decrypt the media cache of Telegram Desktop.

This program will read encrypted Telegram Desktop's media cache and write decrypted data to an output directory.

It may not work for older or newer versions of Telegram Desktop. You should also be aware that the Telegram Desktop cache data is private to you and writing out decrypted data may be risky for leakage.

# Dependencies
* Python 3
* pycryptodome

Pure Python - no C compiler, Qt, or tgcrypto needed, so it also runs on Windows.

# Usage

```
python3 telegram-cache-decryption /path/to/tdata/key_datas /path/to/tdata/user_data -o output_dir
```

`key_datas` and `user_data` live inside Telegram Desktop's `tdata` directory
(e.g. `%APPDATA%\Telegram Desktop\tdata` on Windows, `~/.local/share/TelegramDesktop/tdata` on Linux).
