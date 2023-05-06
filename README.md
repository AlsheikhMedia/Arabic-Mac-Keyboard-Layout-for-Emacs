# Arabic Mac Keyboard Layout for Emacs

To use the `arabic.el` file in your Emacs configuration, follow these steps:

1. Create a directory for your custom Emacs Lisp (Elisp) files if you haven't already. A common location is a directory named `lisp` or `elisp` inside your Emacs configuration directory (usually `~/.emacs.d/`):

   ```
   mkdir ~/.emacs.d/lisp
   ```

2. Save the `arabic.el` file with the modified content to the newly created directory:

   ```
   ~/.emacs.d/lisp/arabic.el
   ```

3. Open your Emacs configuration file (usually `.emacs` in your home directory or `init.el` in `~/.emacs.d/`) and add the following lines to load the custom `arabic.el` file:

   ```elisp
   (add-to-list 'load-path "~/.emacs.d/lisp")
   (require 'arabic)
   ```

   This code adds the `lisp` directory to the `load-path` (which tells Emacs where to look for Elisp files) and then loads the `arabic.el` file.

4. Save your configuration file and restart Emacs for the changes to take effect.

Now you should be able to activate the new input method with `M-x set-input-method RET arabic-mac RET`.
