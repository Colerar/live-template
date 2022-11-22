# live-template

My personal live templates for JetBrains IDEs, including IDEA, CLion, etc.

Official docs for live template: https://www.jetbrains.com/help/idea/using-live-templates.html

File structure(`<name>` denotes variable,
question mark `?` after variable or character denotes it's optional):

```plaintext
<Language>/<TemplateGroup>?-?<TemplateName>.xml
```

Template stores as xml list, it can be parsed by JetBrains IDEs.

## Install

1. Copy a xml file to your clipboard.
   - Open it in your favorite text editor, then select all and copy.
   - If you are using macOS, `cat <template>.xml | pbcopy` is idiomatic.
2. Open IDE Settings/Preferences (Windows: `Ctrl+Alt+S`, macOS: `⌘ + ,`)
3. Goto `Editor -> Live Templates`
4. (Optional) Create a new group based on template group. 
   ![Create new template group](https://user-images.githubusercontent.com/62297254/203260212-ee50795b-b898-4a2c-8f60-c792c6873395.png)
5. Select a group, paste via shortcuts (Windows: `Ctrl+V`, macOS: `⌘ + V`)
6. Enjoy!

## Templates

See README.md of each sub-folder for template information.

- [C++](./C++/README.md)

## License

Distributed under [CC-BY-4.0](./LICENSE).
