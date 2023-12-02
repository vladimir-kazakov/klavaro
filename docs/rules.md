# Mandatory
Every Esperanto keyboard layout must:
- Be based on an existing keyboard layout (first language).  
  _Esperanto was created to be a universal second language. Because of that,
  it must be compatible with the first language._
- Preserve the layout of the first language.  
  _If the layout of the first language already uses keys that Esperanto needs,
  the keys of the first language are more important and must not be changed.
  In other words, Esperanto must find other keys. This ensures that
  the keyboard layout is logical and expected._
- Be stored in the `layouts/xx[-yy]` folder.  
  _There is a lot of languages and layouts, so it makes sense
  to organize layouts accordingly._
  - If it's based on a language that has only one layout, the layout must
    be stored in the `xx` folder, where `xx` is
    the [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
    two-letter language code.
  - If it's based on a language that has multiple layouts, the layout must
    be stored in the `xx-yy` folder, where `yy` is
    the [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
    two-letter country code. `xx` is explained above.
- Be named (file name) as an operating system, the layout is intended for.  
  _There is a lot of operating systems, so it makes sense to organize
  layouts accordingly. For example, `windows.klc`._
- Have the following properties in Microsoft Keyboard Layout Creator.
  - Project name: `xxyyeo`, where `xx` and `yy` come from the name of the folder
    that contains the `windows.klc` file.  
    _This is the name of a DLL file, which will be installed into
    `C:\Windows\System32`. It can't be longer than 8 characters, so it makes
    sense to keep the name as short as possible, and unique for each layout._
  - Description: `original layout, Esperanto`.  
    _For example, if `original layout` is `English (US)`, then the description
    must be `English (US), Esperanto`. It will be shown in the language selector._
  - Company: `Klavaro`.  
    _The project name._
  - Copyright: empty.

Every file in this repository must:
- Have a lowercase name.  
  _For consistency._

# Recommended
It's recommended for every Esperanto keyboard layout:
- To have a quickly accessible `$` (dollar sign: `U+0024`) key.  
  - _It represents one of the popular currencies in the world._
  - _It may be useful in computer programming._
  - _It's logical to map it to `Shift+5` or `AltGr+5`,
    because `5` looks like `S`, but since Esperanto already uses `S` and `Ŝ`,
    `5` is a logical alternative._
- To have a quickly accessible `€` (euro sign: `U+20AC`).  
  - _It represents one of the popular currencies in the world._
  - _Many esperantists are from countries that use this currency._
  - _It's logical to map it to `AltGr+E`, because `E` looks like `€`._