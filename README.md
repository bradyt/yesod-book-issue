Reading from
<https://www.yesodweb.com/book/shakespearean-templates#shakespearean-templates_calling_shakespeare>,
and trying `stack runghc test2.hs`, I get the following issue:

```
$ stack runghc test2.hs 

test2.hs:20:12: error:
    • Exception when trying to run compile-time code:
        "-- @template.lucius
foo { bar: baz }" (line 1, column 1):
unexpected " "
expecting "-->"
CallStack (from HasCallStack):
  error, called at ./Text/Css.hs:136:17 in shakespeare-2.0.12.1-7zylhH6EvxxByWoabG0aiC:Text.Css
      Code: luciusFileDebug "template.lucius"
    • In the untyped splice: $(luciusFileDebug "template.lucius")
```
