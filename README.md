# agnoster-two-lines.zsh-theme

A ZSH theme optimized for people who use:

- Solarized
- Git
- Unicode-compatible fonts and terminals (I use iTerm2 + Menlo)

For Mac users, I highly recommend iTerm 2 + Solarized Dark

# Install
Set agnoster-two-lines theme in your .zshrc
Run ``apply`` script to copy theme to your oh-my-zsh folder

# Compatibility

**NOTE:** In all likelihood, you will need to install a [Powerline-patched font](https://github.com/Lokaltog/powerline-fonts) for this theme to render correctly.

To test if your terminal and font support it, check that all the necessary characters are supported by copying the following command to your terminal: `echo "⮀ ± ⭠ ➦ ✔ ✘ ⚡"`. The result should look like this:

![Character Example](http://cl.ly/content/image/2l3w443z363P/aHR0cDovL2YuY2wubHkvaXRlbXMvM2ozTjJpMDMzTzJNM0ozcDFjMjgvU2NyZWVuJTIwU2hvdCUyMDIwMTItMDktMTQlMjBhdCUyMDEyLjA2LjAyJTIwLnBuZw==)

## What does it show?

- If the previous command failed (✘)
- User @ Hostname (if user is not DEFAULT_USER, which can then be set in your profile)
- Git status
  - Branch (⭠) or detached head (➦)
  - Current branch / SHA1 in detached head state
  - Dirty working directory (±, color change)
- Working directory
- Elevated (root) privileges (⚡)

![Screenshot](https://raw.github.com/gist/3712874/5d28e2d9fe2e4d0a4fda0315ad97bdafa399425c/screenshot.png)

## Future Work

I don't want to clutter it up too much, but I am toying with the idea of adding RVM (ruby version) and n (node.js version) display.

It's currently hideously slow, especially inside a git repo. I guess it's not overly so for comparable themes, but it bugs me, and I'd love to hear ideas about how to improve the performance.

Would be nice for the code to be a bit more sane and re-usable. Something to easily append a section with a given FG/BG, and add the correct opening and closing.

Also the dependency on a powerline-patched font is regrettable, but there's really no way to get that effect without it. Ideally there would be a way to check for compatibility, or maybe even fall back to one of the similar unicode glyphs.
