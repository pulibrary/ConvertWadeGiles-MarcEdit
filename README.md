# ConvertWadeGiles-MarcEdit
MarcEdit plugin for converting Chinese romanization from Wade-Giles to Pinyin.  This is not a batch-processing tool, but can help with the tedious parts of converting the record manually.  The user simply highlights text containing Wade-Giles, runs the plugin, and the text is converted to pinyin.

## Installation/Usage

1. [Download the installer](https://github.com/pulibrary/ConvertWadeGiles-MarcEdit/releases/latest/download/InstallConvertWadeGiles.exe)
  - Compatible with the Windows version of MarcEdit.
  - This plugin does not need to be installed as Administrator.  It should be installed while logged in as the user that will be using the software.
1. Convert the file to MRK format (using the MarcBreaker tool in MarcEdit) and open in MarcEditor.
1. Highlight the text to be converted from Wade-Giles to pinyin.  All the the text must be contained in a single line, though multiple subfields may be highlighted at once.  (But do not highlight the field tag or indicators).
1. Open the "Plugins" menu, and select "ConvertWadeGiles".
1. In the simplest case, the highlighted text will be conveted to pinyin automatically.
  - If any parts of the text are ambiguous between Wade-Giles and pinyin, an alert will pop up after conversion reminding the user to proofread a results.
  - If the text contains an equals sign or ends with a phrase in parenthesis, the tool considers that this may be a translation, and pops a a dialog with additional options, such as deleting the expression, keeping it where it is, or moving it to a 500 field.
