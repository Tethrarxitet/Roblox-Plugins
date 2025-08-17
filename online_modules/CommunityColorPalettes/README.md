# Community Color Palettes
This is the online source for Community Color Palettes!

To make a palette, create a fork of this repo and label it ColorPaletteRequest, and make a copy of `_TemplatePalette.luau`. Fill in the important stuff, and add your colors. Colors can be listed in a few ways:
```luau
{
   {255, 127, 0},             -- Option 1: only the color. Stored as rgb table
   Color3.new(255, 127, 0),   -- Stored as Color3 instance
   "#ff7f00",                 -- Stored as hex color string

   {                                              -- Option 2: color with details
      Color = {255, 127, 0},                      -- You can also show this as the other ones shown before
      Name = "Color name",                        -- Shows up on mouse enter
      Description = "Color description"           -- Shows up after 2 secs of hovering
   }  
}
```
`Color` can also be a `Color3` object or a hex color string. Any color with no name will default to the hex code of the color. Description is optional. More rules:
* Your palette must have more than 16 colors.
* The palette must have a title that references where you got the color palette from.

If you want to create the icon for your palette, download a copy of `ComColPalIconTemplate.rbxlx`. Also do the following:
* Do not change any `Lighting` attributes or add any `Instance`s to it.
* Render quality should be at its lowest.
* Set the color of each `Part` to the name of it (e.g. red, yellow).
    * The Top bricks should be more saturated, whereas the other bricks should be darker (e.g. maroon).
    * If for any reason your color palette doesn't have a main color (which may not give you the best chance of approval), then set all bricks to the nearest color you can find. (e.g. red could be brown, blue could be seafoam green, etc.)
* Resize the window so that the `ViewportSize` of the `Camera` has an aspect ratio of 1:1, and is 640x or higher.

When the viewport has been captured, you can now add the logo of where you got the color palettes from. Make sure that your logo:
* isn't stretched or low quality.
* is the right one. <small><small>Why did we even have to write this?</small></small>
* does not violate Roblox's terms of service.

After that, you may upload and set your new palette `Icon` to your new asset.

### Good examples of icons:
<img width="192" src="https://github.com/user-attachments/assets/a034a9e8-2a86-401f-b6f8-e68bce9bb7de" />

This is exactly what you should do when making icons. Yes, it's used in the plugin, but that doesn't mean I can't use it to set an example! ;)

<img width="192" src="https://github.com/user-attachments/assets/ba1debe8-93f0-4552-be9c-24401967394a" />

Although very niche, this follows the rules and is designed amazingly. The theme doesn't have enough green colors, so the replacement makes sense.

### Bad examples of icons:
<img width="192" src="https://github.com/user-attachments/assets/b6abcc98-07a4-4aed-8806-4f94d656839b" />

Good sizing, but the skybox behind is the wrong one. Also, take a good guess as to what game you're making this for.

<img width="192" src="https://github.com/user-attachments/assets/25b9f32d-83dc-435c-9e0b-00491e4f9cb4" />

4-bit RGBI isn't allowed because the color palette itself is only 16 colors. Also, the camera has been moved, which is not allowed. It's also recommended that the font of the text is either Arial or a font used in the logo, if applicable.
