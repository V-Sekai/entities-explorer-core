# entities-explorer-core

Three GDScript files that the Model Explorer and the obstacle-course twin both use.

| File | What it does |
|---|---|
| `Bintr.gd` | Lists the guest programs (`.elf`) the apps load, with their memory limits, and points the sandbox add-on at the compiled-guest folder. |
| `CardStyle.gd` | The look of the cards in the viewer. |
| `Motion.gd` | The Kimodo clip maker: it asks `motion.elf` and `skintokens.elf` for a clip and puts it on a rig. |

The files keep their paths from the Model Explorer: an app copies them to `res://vsk_model_explorer/core/`.
The history was cut from [V-Sekai/entities-model-explorer](https://github.com/V-Sekai/entities-model-explorer) with `git filter-repo`.

## What this repository does not have

- No `project.godot`: it is not a Godot project, and nothing here has run under Godot on its own.
- No guest programs. `skintokens.elf`, `motion.elf`, `usd.elf`, `headfit.elf` and `persona.elf` are build products of the interactor guest repositories (`tools/fetch_guest_assets.sh` in the explorer fetches them).

## Licence

MIT, see `LICENSE`. Copyright (c) 2022 K. S. Ernest (iFire) Lee and Allen Dang.
