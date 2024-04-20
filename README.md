# cfg sync

create symbolic links between `.cfg` files in an arbitrary folder and individual mod locations, with optional mod whitelisting of specific `.cfg` files.

---

in the assigned configs folder, you can put `.cfg` files that will be linked to each mod in each "mod location". this means that if you edit one `.cfg` file, it will update everywhere!

so for example, if you have `'i:\Quake\Engines\quakespasm-0.95.0_win64\` as a "mod location", it will search for each folder inside of that location, and will symlink `.cfg` files to subfolders such as:

- `quakespasm-0.95.0_win64\ad\example.cfg`
- `quakespasm-0.95.0_win64\copper\example.cfg`
- `quakespasm-0.95.0_win64\alkaline\example.cfg`

`settings.toml`'s configs location is currently `../cfg`, a relative path, but it can be whatever you want, like `r:\Quake\quake_configs`

> [!NOTE]
> if you have a `.cfg` you only want in certain mods, you can add it to a whitelist under `[limit]` in `settings.toml`

> [!NOTE]
> see `settings.toml` for an example configuration
