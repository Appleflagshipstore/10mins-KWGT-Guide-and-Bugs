10 mins Kustom Guide for Newbie by Newbie\
KWGT Known Limits and Known Issues
===========================================================================
By Sappurit (Joined Kustom universe at FEB 2021)

---

Kustom is a very powerful app on Android OS. You can create or design widget wallpaper by following your imagination. With all due respect, Kustom is not straightforward. There are many known limits and known Issues that newbie should know before designing any complex preset.

## Understand the GUI

- Available spaces are a list of your Kustom widgets on the home screen. (Why not rename it to Widget Lists ?!!?)

  ![Available spaces](https://s3.imgcdn.dev/ITFHu.png)

- Widget that never exports and reload presets will be named with some sequence number.

- You can't rename the widget name directly. To change a widget name, you have to export the widget to a new preset and reload that preset over your current widget again.

- No browse button when export preset. Manual typing is only your choice. Be careful, no overwritten warning popup dialog. It's good to export new names and reload the present of every widget. It will remember the export info. But sometimes it shows the other widget info.

  ![No browse button](https://s3.imgcdn.dev/ITXCL.png)

- Some properties, Edit button is hidden in the three dots (⋮) button. But you have to select the item first.


## Kustom Known Limits and Known Issues

- Global variables have a limit of 8 characters.

- You can't rename global variable names.

- When editing a global variable description, it will clear the value.

- In Komponent, you can't edit the global variable description.

- You can use the same global formula variable only 4 times in a formula.

- Move items into the Overlap group, Stack group and Komponent will lose the position settings. Because it will work as padding instead of X/Y offsets.

- Hard to combine string and numeric in the if() function. You have to split if() or use tc(reg).\
  [add image]

- wg() sometimes returns an invalid numeric. You have to add + 0 at the end of function.\
  [add image]

- wg() xpath don’t support html unclosed tag. Eg. `<img>`

- Font property doesn’t have a formula button. You have to use a global font variable.

- Global font variable formulas need to return as a pointer to the kustom font file.

      kfile://org.kustom.provider/fonts/Roboto-Black.ttf
      kfile://org.kustom.provider/fonts/Roboto-Bold.ttf
      kfile://org.kustom.provider/fonts/Roboto-Light.ttf
      kfile://org.kustom.provider/fonts/Roboto-Medium.ttf
      kfile://org.kustom.provider/fonts/Roboto-Regular.ttf
      kfile://org.kustom.provider/fonts/Roboto-Thin.ttf
      kfile://org.kustom.provider/fonts/RobotoCondensed-Bold.ttf
      kfile://org.kustom.provider/fonts/RobotoCondensed-Light.ttf
      kfile://org.kustom.provider/fonts/RobotoCondensed-Regular.ttf
      
  ![Global font variable formulas](https://s3.imgcdn.dev/ITg7a.png)

- Invalid Width when using Text box’s Type property as Fit Width. Width is smaller than usual.

  ![Invalid Width](https://s3.imgcdn.dev/ITqxB.png)
  
- Beware confusion. Symbol of Text item use the same as font property. I would change to the big T that will be matched with the global text variable.

  ![Text Symbol](https://s3.imgcdn.dev/ITELw.png)
  
- No NumToStr() and StrToNum() functions. There is a problem when concatenating numeric strings with numeric. Especially in if() function. The easy way is split the if() function.

  ![Concatenating](https://s3.imgcdn.dev/IToUT.png)
  
  
