# Travel Posters Collection Design

## Goal

Add a new prompt collection named "Travel Posters" based on the provided geometric travel poster guide, while reorganizing the existing standalone prompt examples into a clearer collection structure.

## Collection Structure

The prompt area will become collection-based:

- `docs/prompts/README.md` becomes the top-level prompt collection index.
- `docs/prompts/travel-posters/` contains the new Travel Posters guide, reusable master template, and 14 city prompt files.
- `docs/prompts/visual-illusions/` contains the existing 9 long-form illusion and scale prompts.
- `examples/prompts/travel-posters/` contains generated poster examples.
- `examples/prompts/visual-illusions/` contains the existing generated examples after relocation.

## Travel Posters Content

Each Travel Posters city file will contain a complete copy-paste-ready prompt. The wording will be rewritten and tightened from the source PDF rather than copied verbatim, while preserving the central design system:

- Vertical 2:3 or 3:4 poster format.
- One small uppercase city name at the top.
- Lower-half cityscape built around one or two recognizable landmarks.
- 70% recognizable landmark and architecture, 30% geometric abstraction.
- Muted museum-print palette, subtle handmade texture, no photorealism or poster clutter.

The collection README will include the usage method, the one-second recognizability test, and a table linking every city prompt to its generated example image.

## Existing Prompt Reorganization

The existing 9 prompt files and images will move into the "Visual Illusions" collection. Their content should remain functionally unchanged except for image link paths and collection index links.

## Verification

Verification is file-based:

- Confirm all expected Markdown files exist.
- Confirm all referenced example images exist.
- Search for broken old image paths.
- Review git diff to ensure only intended documentation and example assets changed.
