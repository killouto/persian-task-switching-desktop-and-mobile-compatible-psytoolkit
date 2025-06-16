# Task Switching (Persian)

This folder contains a translated and customized version of a **Task Switching** paradigm, implemented in [PsyToolkit](https://www.psytoolkit.org/). The task is adapted for both **mobile** and **desktop** platforms, with all materials presented in **Persian**.

## Purpose

This experiment evaluates **cognitive flexibility**, particularly the cost of switching between tasks. Participants alternate between two tasks: identifying shapes or counting filled elements. The experiment compares pure (single-task) and mixed (interleaved-task) blocks to calculate **switch costs** and **mixing costs**.

## Attribution

Original experiment design and script by Gijsbert Stoet, PhD , PsyToolkit developer.  
**Translated and adapted into Persian by Sepehr Moraghebi**, with mobile and desktop compatibility via PsyToolkit.

## File Contents

- `code.psy`: The full experiment script
- `stimuli/`: Folder containing visual stimuli for shape and fill tasks
- `README.md`: This file

## Output Data Format

Each trial in the experiment generates one row with **9 columns**:

| Column | Description |
|--------|-------------|
| 1 | **Block name** (e.g., `switchpureshape`, `switchmixedshapefilling`) |
| 2 | **Stimulus index**: Row number from the corresponding task table |
| 3 | **Task type**: Either `shape` or `fill` |
| 4 | **Stimulus congruency**: `congruent` or `incongruent` |
| 5 | **Correct response side**: `left` or `right` |
| 6 | **Accuracy**: `1 = correct`, `2 = incorrect` |
| 7 | **Reaction time** in milliseconds |
| 8 | **Block type**: `1 = pure block`, `2 = mixed block` |
| 9 | **Switch type**: `1 = repeat trial`, `2 = switch trial` |

## Notes

- Task-switching cost is calculated from RT differences between repeat and switch trials in mixed blocks.
- Mixing cost is calculated from RT differences between mixed and pure blocks.
- Feedback at the end of the task is based on these metrics.

## Repository

This experiment is part of the full project:  
🔗 [killouto/cognitive-tasks-persian-mobile-desktop](https://github.com/killouto/cognitive-tasks-persian-mobile-desktop)

## License

This project is licensed under the MIT License. See the [LICENSE](../../LICENSE) file for details.
