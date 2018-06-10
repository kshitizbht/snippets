
### VS Code

1. Install VSCode
2. Add Eclipse Keymap, Go, Java Extension Pack, Markdownlint
3. Reload once last extension is loaded
   
Java pack may change .project and .prefs to convert all Java Project to Maven Nature, to overwrite it, you can,
```
   git checkout -- $(git diff --name-only  | grep .project)
   git checkout -- $(git diff --name-only  | grep .prefs)
```

### Commands

Since we mapped Eclipse Keymap, CMD + Shift + R , CMD + L and other Eclipse command work as is


Command|Usage
---- | -----
⌘P|Workspace search
⌘⇧P|Command search


### Links
https://code.visualstudio.com/docs/getstarted/userinterface
