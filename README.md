# Support for golang was added based on the configuration of Purcell

## Installation

To install, clone this repo to `~/.emacs.d`, i.e. ensure that the
`init.el` contained in this repo ends up at `~/.emacs.d/init.el`:

```
git clone https://github.com/lzt1226/emacs-config.git ~/.emacs.d
```

Upon starting up Emacs for the first time, further third-party
packages will be automatically downloaded and installed. If you
encounter any errors at that stage, try restarting Emacs, and possibly
running `M-x package-refresh-contents` before doing so.


## Support
- [x] Ruby / Ruby on Rails
- [x] CSS / LESS / SASS / SCSS
- [x] HAML / Markdown / Textile / ERB
- [x] Clojure (with Cider and nRepl)
- [x] Javascript / Coffeescript
- [x] Python
- [x] PHP
- [x] Haskell
- [x] Elm
- [x] Erlang
- [x] Common Lisp (with Slime)
- [x] `Important` Golang

## Step
* Install `go-mode`,`company` and `company-go`, `m-x package-install` directly
* go get -u github.com/nsf/gocode
* go get -u github.com/rogpeppe/godef
* go get -u github.com/dougm/goflymake
	* Modify the file `.emacs.d/lisp/init-go.el`
	* (add-to-list 'load-path "$GOPATH/src/github.com/dougm/goflymake")(require 'go-flymake)
	* (add-to-list 'load-path "$GOPATH/src/github.com/dougm/goflymake")(require 'go-flycheck)
	* Replace `$GOPATH` is `your gopath`
* `neotree` has supported
	* Shortcut key id `F8`

## Thanks
Thanks [Purcell](https://github.com/purcell/emacs.d)



