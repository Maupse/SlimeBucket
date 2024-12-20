# Elixir Terminal Translator
A Command Line Interface that uses google API to translate text inside the terminal, written in Elixir.  
[View on Github](https://github.com/Maupse/elixir_terminal_translator)

## Installation

Using scoop you can add the Bucket https://github.com/Maupse/SlimeBucket
```pwsh
> scoop bucket add SlimeBucket "https://github.com/maupse/SlimeBucket"
```

Then just run
```pwsh
> scoop install elixir-terminal-translator
```

## Basic Usage

```pwsh
> tl --help
```

```
--in, -i <ISO-639-two-letter-language-code> sets the input language for the translator 
 Example: -i en for english
--out, -o <ISO-639-two-letter-language-code> sets the output language for the translator 
 Example: -o de for german
--version, -v Boolean flag, prints out the version of the program
--path, -p <path/to/out_dir> The directory where the translated file goes, will be named translation_<Iso-639-letters>
--help, -h Boolean flag, explains every option and argument given, if there are no arguments explains everything
--translator, -t google sets the translator you want to translate with (only google available for now)
--set-api-key, -s <API-KEY>, sets API key for the current translator

Fast syntax is: tl :<out-code> :<in-code> flags text (if there is one it will be counted as out)
You can set flags with --this-is-a-flag <argument> (no arguments for boolean flags)
Flags have to come before the text, only the head gets parsed
```
