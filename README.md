# Marketing brief

**https://rahman-oxcel.github.io/marketing-brief/**

The page is AES-256 encrypted ([StatiCrypt](https://github.com/robinmoisson/staticrypt)).
Ask Rahman for the password. This repo is public, so only the encrypted output ships;
the source stays local in `src/` (git-ignored).

## Rebuilding

```
npx staticrypt src/brief.html -p "<password>" -d build --short --remember 30 --template-title "Oxcel marketing brief" --template-instructions "Enter the password Rahman gave you." --template-placeholder "Password" --template-button "Open the brief" --template-remember "Remember me on this device for 30 days" --template-error "That password didn't work. Check it with Rahman." --template-color-primary "#001732" --template-color-secondary "#F5F6F8"
cp build/brief.html index.html
```

Keep `.staticrypt.json` (the salt) so a rebuild with the same password keeps "remember me" working.
