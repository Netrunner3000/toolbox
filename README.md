# Toolbox

Small utilities kept apart from the lab's standalone apps — none of these is a product
in its own right, launched separately with its own window and lifecycle. Each is its own
git repo, included here as a submodule.

- `unblock_tracker/` — PySide6 "Unblock Tracker" app; watches whether an Instagram profile
  has unblocked you.
- `convert_epub/` — "Ebook Converter.app"; any-format ebook/doc conversion via Calibre.
- `image_tools/` — small image-prep utilities (`dpi/`, `rename/`, `move/`).

A proper GUI front end for Toolbox (its own small launcher, in the spirit of Lab Hub) is
planned but not built yet.

## Cloning

Submodules aren't fetched by a plain `git clone`. Use:

    git clone --recurse-submodules <this repo's url>

or, on an existing checkout:

    git submodule update --init --recursive
