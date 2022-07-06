# ASP.NET RegEx for Visual Studio 2019

Tested 2022/05/03 in the IDE and <https://regex101.com>

Used in the .aspx page with the **RegularExpressionValidator** Class to manage textboxes input.

## Construction

1. To allow lower and upper case words from a to z, not spaces

            ^[a-zA-Z]*$

2. To don't allow numbers from 0 to 9 and symbols

            ^[^0-9\\|!¡@·#$~%&¬/()=¿?'^`\[\]+*¨´{}ç,;.:_-]*$

3. To allow words, no spaces, no numbers or symbols

            ^[a-zA-Z]*$[^0-9\\|!¡@·#$~%&¬/()=¿?'^`\[\]+*¨´{}ç,;.:_-]*$

4. To allow words with a max lenght of 50 characters, no spaces, no numbers or symbols

            ^[a-zA-Z]{0,50}$[^0-9\\|!¡@·#$~%&¬/()=¿?'^`\[\]+*¨´{}ç,;.:_-]*$

This symbols are don't recognized and gives errors when inserted in the Regular Expression:
_º ª " > <_
