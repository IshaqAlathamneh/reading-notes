# CSS
CSS stands for Cascading Style Sheets.
## What's CSS do?
* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
* Different types of selectors allow you to target your rules at different elements.
* Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document, although they may appear within an HTML page.

## Color

*** Foreground Color ***
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
1. rgb values: example: rgb(100,100,90)
1. hex codes: For example: #ee3e80
1. color names:  For example: DarkCyan

*** Background color *** 
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
You can specify your choice of background color in the same three ways you can specify foreground colors.
*** Understanding Color ***
Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.
* Computer monitors are made up of thousands of tiny squares called pixels.
* When the screen is not turned on, it's black because it's not emitting any light. When it's on, each pixel can be a different color, creating a picture.
* Color picking tools are available in image editing programs like Photoshop and GIMP.


**RGB Values:** Values for red, green, and blue are expressed as numbers between 0 and 255.

**Hex Codes:**Hex values represent values for red, green, and blue in hexadecimal code.
**Color Names**

**Hue:** Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.
**Saturation:** Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.
**Brightness:** Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark.
## Contrast
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
![contrast](data:image/png;base64,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)


 ## CSS3: Opacity
 CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0
 ## CSS3: HSL Colors
 CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.
 * hue
Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.
* saturation
Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.
* lightness
Lightness is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity.
## CSS3: HSL & HSLA
The hsl color property has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for: HUE and saturation and lightness
ALPHA: This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.