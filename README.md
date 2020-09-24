![vim-polyglot](https://i.imgur.com/9RxQK6k.png)

![build](https://github.com/sheerun/vim-polyglot/workflows/Vim%20Polyglot%20CI/badge.svg) [![Maintenance](https://img.shields.io/badge/maintained%20since-2013-yes)]()

A collection of language packs for Vim.

> One to rule them all, one to find them, one to bring them all and in the darkness bind them.

- It **won't affect your startup time**, as scripts are loaded only on demand\*.
- It **installs and updates 120+ times faster** than the <!--Package Count-->201<!--/Package Count--> packages it consists of.
- It is more secure because scripts loaded for all extensions are generated by vim-polyglot (ftdetect).
- Solid syntax and indentation support (other features skipped). Only the best language packs.
- All unnecessary files are ignored (like enormous documentation from php support).
- Automatically detect indentation (includes performance-optimized version of [vim-sleuth](https://github.com/tpope/vim-sleuth))
- Each build is tested by automated vimrunner script on CI. See `spec` directory.

\*To be completely honest, optimized `ftdetect` script takes around `20ms` to load.

## Installation

1. Install [Pathogen](https://github.com/tpope/vim-pathogen), [Vundle](https://github.com/VundleVim/Vundle.vim), [NeoBundle](https://github.com/Shougo/neobundle.vim), or [Plug](https://github.com/junegunn/vim-plug) package manager for Vim.
2. Use this repository as submodule or package.

For example when using [Plug](https://github.com/junegunn/vim-plug):

```
Plug 'sheerun/vim-polyglot'
```

Optionally download one of the [releases](https://github.com/sheerun/vim-polyglot/releases) and unpack it directly under `~/.vim` directory.

You can also use Vim 8 built-in package manager:

```
mkdir -p ~/.vim/pack/default/start
git clone https://github.com/sheerun/vim-polyglot ~/.vim/pack/default/start/vim-polyglot
```

NOTE: Not all features of individual language packs are available. We strip them from functionality slowing vim startup (for example we ignore `plugins` folder that is loaded regardless of file type, instead we prefer `ftplugin` which is loaded lazily).

If you need full functionality of any plugin, please use it directly with your plugin manager.

## Language packs

<!--Language Packs-->
- [8th](https://github.com/vim/vim/tree/master/runtime)
- [a2ps](https://github.com/vim/vim/tree/master/runtime)
- [a65](https://github.com/vim/vim/tree/master/runtime)
- [aap](https://github.com/vim/vim/tree/master/runtime)
- [abap](https://github.com/vim/vim/tree/master/runtime)
- [abaqus](https://github.com/vim/vim/tree/master/runtime)
- [abc](https://github.com/vim/vim/tree/master/runtime)
- [abel](https://github.com/vim/vim/tree/master/runtime)
- [acedb](https://github.com/vim/vim/tree/master/runtime)
- [acpiasl](https://github.com/martinlroth/vim-acpi-asl)
- [ada](https://github.com/vim/vim/tree/master/runtime)
- [ahdl](https://github.com/vim/vim/tree/master/runtime)
- [aidl](https://github.com/vim/vim/tree/master/runtime)
- [alsaconf](https://github.com/vim/vim/tree/master/runtime)
- [aml](https://github.com/vim/vim/tree/master/runtime)
- [ampl](https://github.com/vim/vim/tree/master/runtime)
- [ansible](https://github.com/pearofducks/ansible-vim)
- [ant](https://github.com/vim/vim/tree/master/runtime)
- [apache](https://github.com/vim/vim/tree/master/runtime)
- [apiblueprint](https://github.com/kylef/apiblueprint.vim)
- [applescript](https://github.com/mityu/vim-applescript)
- [aptconf](https://github.com/vim/vim/tree/master/runtime)
- [arch](https://github.com/vim/vim/tree/master/runtime)
- [arduino](https://github.com/sudar/vim-arduino-syntax)
- [art](https://github.com/vim/vim/tree/master/runtime)
- [asciidoc](https://github.com/asciidoc/vim-asciidoc)
- [asn](https://github.com/vim/vim/tree/master/runtime)
- [aspperl](https://github.com/vim/vim/tree/master/runtime)
- [aspvbs](https://github.com/vim/vim/tree/master/runtime)
- [atlas](https://github.com/vim/vim/tree/master/runtime)
- [autohotkey](https://github.com/hnamikaw/vim-autohotkey)
- [autoit](https://github.com/vim/vim/tree/master/runtime)
- [automake](https://github.com/vim/vim/tree/master/runtime)
- [ave](https://github.com/vim/vim/tree/master/runtime)
- [awk](https://github.com/vim/vim/tree/master/runtime)
- [basic](https://github.com/vim/vim/tree/master/runtime)
- [blade](https://github.com/jwalton512/vim-blade)
- [brewfile](https://github.com/bfontaine/Brewfile.vim)
- [bzl](https://github.com/vim/vim/tree/master/runtime)
- [c/c++](https://github.com/vim-jp/vim-cpp)
- [caddyfile](https://github.com/isobit/vim-caddyfile)
- [carp](https://github.com/hellerve/carp-vim)
- [cjsx](https://github.com/mtscout6/vim-cjsx)
- [clojure](https://github.com/guns/vim-clojure-static)
- [cmake](https://github.com/pboettch/vim-cmake-syntax)
- [coffee-script](https://github.com/kchmck/vim-coffee-script)
- [cpp-modern](https://github.com/bfrg/vim-cpp-modern)
- [cql](https://github.com/elubow/cql-vim)
- [cryptol](https://github.com/victoredwardocallaghan/cryptol.vim)
- [crystal](https://github.com/rhysd/vim-crystal)
- [csv](https://github.com/chrisbra/csv.vim)
- [cucumber](https://github.com/tpope/vim-cucumber)
- [cue](https://github.com/mgrabovsky/vim-cuesheet)
- [dart](https://github.com/dart-lang/dart-vim-plugin)
- [dhall](https://github.com/vmchale/dhall-vim)
- [dlang](https://github.com/JesseKPhillips/d.vim)
- [dockerfile](https://github.com/ekalinin/Dockerfile.vim)
- [dosini](https://github.com/vim/vim/tree/master/runtime)
- [elf](https://github.com/vim/vim/tree/master/runtime)
- [elixir](https://github.com/elixir-lang/vim-elixir)
- [elm](https://github.com/andys8/vim-elm-syntax)
- [emberscript](https://github.com/yalesov/vim-ember-script)
- [emblem](https://github.com/yalesov/vim-emblem)
- [erlang](https://github.com/vim-erlang/vim-erlang-runtime)
- [fennel](https://github.com/bakpakin/fennel.vim)
- [ferm](https://github.com/vim-scripts/ferm.vim)
- [fish](https://github.com/georgewitteman/vim-fish)
- [flatbuffers](https://github.com/dcharbon/vim-flatbuffers)
- [forth](https://github.com/vim/vim/tree/master/runtime)
- [fsharp](https://github.com/ionide/Ionide-vim)
- [gdscript](https://github.com/calviken/vim-gdscript3)
- [git](https://github.com/tpope/vim-git)
- [gitignore](https://github.com/rdolgushin/gitignore.vim)
- [glsl](https://github.com/tikhomirov/vim-glsl)
- [gmpl](https://github.com/maelvalais/gmpl.vim)
- [gnuplot](https://github.com/vim-scripts/gnuplot-syntax-highlighting)
- [go](https://github.com/fatih/vim-go)
- [gradle](https://github.com/tfnico/vim-gradle)
- [graphql](https://github.com/jparise/vim-graphql)
- [groovy](https://github.com/vim/vim/tree/master/runtime)
- [grub](https://github.com/vim/vim/tree/master/runtime)
- [haml](https://github.com/tpope/vim-haml)
- [handlebars](https://github.com/mustache/vim-mustache-handlebars)
- [haproxy](https://github.com/CH-DanReif/haproxy.vim)
- [haskell](https://github.com/neovimhaskell/haskell-vim)
- [haxe](https://github.com/yaymukund/vim-haxe)
- [hcl](https://github.com/b4b4r07/vim-hcl)
- [helm](https://github.com/towolf/vim-helm)
- [help](https://github.com/neovim/neovim/tree/master/runtime)
- [hive](https://github.com/zebradil/hive.vim)
- [html5](https://github.com/othree/html5.vim)
- [htmldjango](https://github.com/vim/vim/tree/master/runtime)
- [i3](https://github.com/mboughaba/i3config.vim)
- [icalendar](https://github.com/chutzpah/icalendar.vim)
- [idris2](https://github.com/edwinb/idris2-vim)
- [idris](https://github.com/idris-hackers/idris-vim)
- [ion](https://github.com/vmchale/ion-vim)
- [javascript-sql](https://github.com/statico/vim-javascript-sql)
- [javascript](https://github.com/pangloss/vim-javascript)
- [jenkins](https://github.com/martinda/Jenkinsfile-vim-syntax)
- [jq](https://github.com/vito-c/jq.vim)
- [json5](https://github.com/GutenYe/json5.vim)
- [json](https://github.com/elzr/vim-json)
- [jsonnet](https://github.com/google/vim-jsonnet)
- [jst](https://github.com/briancollins/vim-jst)
- [jsx](https://github.com/MaxMEllon/vim-jsx-pretty)
- [julia](https://github.com/JuliaEditorSupport/julia-vim)
- [kotlin](https://github.com/udalov/kotlin-vim)
- [ledger](https://github.com/ledger/vim-ledger)
- [less](https://github.com/groenewege/vim-less)
- [lilypond](https://github.com/anowlcalledjosh/vim-lilypond)
- [livescript](https://github.com/gkz/vim-ls)
- [llvm](https://github.com/rhysd/vim-llvm)
- [log](https://github.com/MTDL9/vim-log-highlighting)
- [lua](https://github.com/tbastos/vim-lua)
- [m4](https://github.com/vim/vim/tree/master/runtime)
- [mako](https://github.com/sophacles/vim-bundle-mako)
- [markdown](https://github.com/plasticboy/vim-markdown)
- [mathematica](https://github.com/voldikss/vim-mma)
- [mdx](https://github.com/jxnblk/vim-mdx-js)
- [meson](https://github.com/mesonbuild/meson/tree/master/data/syntax-highlighting/vim)
- [moonscript](https://github.com/leafo/moonscript-vim)
- [murphi](https://github.com/vim/vim/tree/master/runtime)
- [nginx](https://github.com/chr4/nginx.vim)
- [nim](https://github.com/zah/nim.vim)
- [nix](https://github.com/LnL7/vim-nix)
- [objc](https://github.com/b4winckler/vim-objc)
- [ocaml](https://github.com/rgrinberg/vim-ocaml)
- [octave](https://github.com/McSinyx/vim-octave)
- [odin](https://github.com/Tetralux/odin.vim)
- [opencl](https://github.com/petRUShka/vim-opencl)
- [perl](https://github.com/vim-perl/vim-perl)
- [pgsql](https://github.com/lifepillar/pgsql.vim)
- [php](https://github.com/StanAngeloff/php.vim)
- [plantuml](https://github.com/aklt/plantuml-syntax)
- [pony](https://github.com/jakwings/vim-pony)
- [powershell](https://github.com/PProvost/vim-ps1)
- [prolog](https://github.com/vim/vim/tree/master/runtime)
- [protobuf](https://github.com/uarun/vim-protobuf)
- [pug](https://github.com/digitaltoad/vim-pug)
- [puppet](https://github.com/rodjek/vim-puppet)
- [purescript](https://github.com/purescript-contrib/purescript-vim)
- [python-compiler](https://github.com/aliev/vim-compiler-python)
- [python-indent](https://github.com/Vimjas/vim-python-pep8-indent)
- [python](https://github.com/vim-python/python-syntax)
- [qmake](https://github.com/artoj/qmake-syntax-vim)
- [qml](https://github.com/peterhoeg/vim-qml)
- [r-lang](https://github.com/vim-scripts/R.vim)
- [racket](https://github.com/wlangstroth/vim-racket)
- [ragel](https://github.com/jneen/ragel.vim)
- [raku](https://github.com/Raku/vim-raku)
- [raml](https://github.com/IN3D/vim-raml)
- [razor](https://github.com/adamclerk/vim-razor)
- [reason](https://github.com/reasonml-editor/vim-reason-plus)
- [requirements](https://github.com/raimon49/requirements.txt.vim)
- [rspec](https://github.com/keith/rspec.vim)
- [rst](https://github.com/marshallward/vim-restructuredtext)
- [ruby](https://github.com/vim-ruby/vim-ruby)
- [rust](https://github.com/rust-lang/rust.vim)
- [sbt](https://github.com/derekwyatt/vim-sbt)
- [scala](https://github.com/derekwyatt/vim-scala)
- [scss](https://github.com/cakebaker/scss-syntax.vim)
- [sh](https://github.com/arzg/vim-sh)
- [slim](https://github.com/slim-template/vim-slim)
- [slime](https://github.com/slime-lang/vim-slime-syntax)
- [smt2](https://github.com/bohlender/vim-smt2)
- [solidity](https://github.com/tomlion/vim-solidity)
- [stylus](https://github.com/wavded/vim-stylus)
- [svelte](https://github.com/evanleck/vim-svelte/tree/main)
- [svg-indent](https://github.com/jasonshell/vim-svg-indent)
- [svg](https://github.com/vim-scripts/svg.vim)
- [swift](https://github.com/keith/swift.vim)
- [sxhkd](https://github.com/baskerville/vim-sxhkdrc)
- [systemd](https://github.com/wgwoods/vim-systemd-syntax)
- [tads](https://github.com/vim/vim/tree/master/runtime)
- [terraform](https://github.com/hashivim/vim-terraform)
- [textile](https://github.com/timcharper/textile.vim)
- [thrift](https://github.com/solarnz/thrift.vim)
- [tmux](https://github.com/ericpruitt/tmux.vim/tree/master/vim)
- [toml](https://github.com/cespare/vim-toml)
- [tptp](https://github.com/c-cube/vim-tptp)
- [trasys](https://github.com/vim/vim/tree/master/runtime)
- [twig](https://github.com/lumiliet/vim-twig)
- [typescript](https://github.com/HerringtonDarkholme/yats.vim)
- [unison](https://github.com/unisonweb/unison/tree/trunk/editor-support/vim)
- [v](https://github.com/ollykel/v-vim)
- [vala](https://github.com/arrufat/vala.vim)
- [vbnet](https://github.com/vim-scripts/vbnet.vim)
- [vcl](https://github.com/smerrill/vcl-vim-plugin)
- [velocity](https://github.com/lepture/vim-velocity)
- [visual-basic](https://github.com/vim/vim/tree/master/runtime)
- [vmasm](https://github.com/vim/vim/tree/master/runtime)
- [vue](https://github.com/posva/vim-vue)
- [xdc](https://github.com/amal-khailtash/vim-xdc-syntax)
- [xml](https://github.com/amadeus/vim-xml)
- [xsl](https://github.com/vim-scripts/XSLT-syntax)
- [yaml](https://github.com/vim/vim/tree/df44a27b53586fccfc6a3aedc89061fdd9a515ff/runtime)
- [yard](https://github.com/noprompt/vim-yardoc)
- [zephir](https://github.com/xwsoul/vim-zephir)
- [zig](https://github.com/ziglang/zig.vim)
- [zinit](https://github.com/zinit-zsh/zplugin-vim-syntax)
<!--/Language Packs-->

## Updating

You can either wait for new patch release with updates or run `make` by yourself.

## Troubleshooting

Please make sure you have `syntax on` in your `.vimrc` (or use something like [sheerun/vimrc](https://github.com/sheerun/vimrc))

Individual language packs can be disabled by setting `g:polyglot_disabled` as follows:

```vim
let g:polyglot_disabled = ['markdown']
```

The list of available languages to disable is shown above.

*Please declare this variable before polyglot is loaded (at the top of .vimrc)*

If you wish to use filetype detection by Vim Polyglot but you'd like to use your own syntax-highlighting plugin, you can append `.plugin` to disabled entry, like below. Disabling Vim Polyglot filetype plugin won't disable native Vim filetype plugin.

```vim
let g:polyglot_disabled = ['markdown.plugin']
```

Please note that disabling a language won't make in your vim startup any faster / slower (only for specific this specific filetype). All plugins are lazily loaded only when they are really needed. 

Vim Polyglot tries to automatically detect indentation settings (just like vim-sleuth). If this feature is not working for you for some reason, please file an issue and disable it temporarily with:

```vim
let g:polyglot_disabled = ['autoindent']
```

## Contributing

Language packs are periodically updated using automated `scripts/build` script.

Feel free to add your language to `packages.yaml` + `heuristics.yaml`, and send pull-request. You can run `make test` to run rough tests. And `make dev` for easy development.

## License

See linked repositories for detailed license information. This repository is MIT-licensed.
