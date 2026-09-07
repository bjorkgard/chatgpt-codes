# AI Map Animations

Two-step prompts for generating a realistic map diorama still image, then turning that still into a short cinematic map animation.

## How To Use

1. Paste Step 1 into Gemini to create the still frame.
2. Replace the bracketed placeholders with the country, city, monument, landscape details, and materials you want.
3. Upload the generated still frame to Google Flow.
4. Paste Step 2 into Google Flow and replace the focal-point placeholder with the same monument.
5. Keep the animation short and stable so the map, diorama, and landmark remain recognizable.

## Prompt Files

| Prompt | Theme | Example |
|---|---|---|
| [AI Map Animation](01-ai-map-animation.md) | Miniature 3D city diorama rising from a geographic map, then converted into a cinematic drone orbit | ![New York AI map animation example](../../../examples/prompts/ai-map-animations/01-new-york-map-diorama.png) |

## Usage Notes

This workflow works best when the first frame is geographically clear and the second prompt asks for controlled motion. Name the main landmark, nearby water, architectural style, parks, and materials so the image model has enough specific structure to build from.
