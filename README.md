# Remove_empty_headings Extension For Quarto

Drafts produced by Saros or other automated systems may include empty headings. This filter removes them.

## Installing

```bash
quarto add NIFU-NO/remove_empty_headings
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

## Using

Add to your YAML header of the document:
```yaml
filters: 
  - remove_empty_headings
```

Or alternatively (experimental) in your `_quarto.yaml` for a website or book project.
```yaml
project:
  pre-render:
    remove_empty_headings.lua
```


## Example

Here is the source code for a minimal example: [example.qmd](example.qmd).

