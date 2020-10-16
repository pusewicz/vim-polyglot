![vim-polyglot](https://i.imgur.com/9RxQK6k.png)

![build](https://github.com/sheerun/vim-polyglot/workflows/Vim%20Polyglot%20CI/badge.svg) [![Maintenance](https://img.shields.io/badge/maintained%20since-2013-yes)]()

A collection of language packs for Vim.

> One to rule them all, one to find them, one to bring them all and in the darkness bind them.

- It **won't affect your startup time**, as scripts are loaded only on demand\*.
- It **installs and updates 120+ times faster** than the <!--Package Count-->593<!--/Package Count--> packages it consists of.
- It is more secure because scripts loaded for all extensions are generated by vim-polyglot (ftdetect).
- Solid syntax and indentation support (other features skipped). Only the best language packs.
- All unnecessary files are ignored (like enormous documentation from php support).
- Automatically detect indentation (includes performance-optimized version of [vim-sleuth](https://github.com/tpope/vim-sleuth))
- Each build is tested by automated vimrunner script on CI. See `spec` directory.

\*To be completely honest, optimized `ftdetect` script takes around `10ms` to load.

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
git clone --depth 1 https://github.com/sheerun/vim-polyglot ~/.vim/pack/plugins/start/vim-polyglot
```

NOTE: Not all features of individual language packs are available. We strip them from functionality slowing vim startup (for example we ignore `plugins` folder that is loaded regardless of file type, instead we prefer `ftplugin` which is loaded lazily).

If you need full functionality of any plugin, please use it directly with your plugin manager.

## Language packs

On top of all language packs from [vim repository](https://github.com/vim/vim/tree/master/runtime), vim-polyglot includes:

<!--Language Packs-->
- [acpiasl](https://github.com/martinlroth/vim-acpi-asl) (asl filetype)
- [ansible](https://github.com/pearofducks/ansible-vim) (yaml.ansible filetype)
- [apiblueprint](https://github.com/kylef/apiblueprint.vim) (apiblueprint filetype)
- [applescript](https://github.com/mityu/vim-applescript) (applescript filetype)
- [arduino](https://github.com/sudar/vim-arduino-syntax) (arduino filetype)
- [asciidoc](https://github.com/asciidoc/vim-asciidoc) (asciidoc filetype)
- [autohotkey](https://github.com/hnamikaw/vim-autohotkey) (autohotkey filetype)
- [blade](https://github.com/jwalton512/vim-blade) (blade filetype)
- [brewfile](https://github.com/bfontaine/Brewfile.vim) (brewfile filetype)
- [c/c++](https://github.com/vim-jp/vim-cpp) (cpp,  and c filetypes)
- [caddyfile](https://github.com/isobit/vim-caddyfile) (caddyfile filetype)
- [carp](https://github.com/hellerve/carp-vim) (carp filetype)
- [cjsx](https://github.com/mtscout6/vim-cjsx)
- [clojure](https://github.com/guns/vim-clojure-static) (clojure filetype)
- [cmake](https://github.com/pboettch/vim-cmake-syntax) (cmake filetype)
- [coffee-script](https://github.com/kchmck/vim-coffee-script) (coffee, litcoffe and litcoffee filetypes)
- [cpp-modern](https://github.com/bfrg/vim-cpp-modern)
- [cql](https://github.com/elubow/cql-vim) (cql filetype)
- [cryptol](https://github.com/victoredwardocallaghan/cryptol.vim) (cryptol filetype)
- [crystal](https://github.com/rhysd/vim-crystal) (crystal, ecrysta and ecrystal filetypes)
- [csv](https://github.com/chrisbra/csv.vim) (csv filetype)
- [cucumber](https://github.com/tpope/vim-cucumber) (cucumber filetype)
- [cue](https://github.com/mgrabovsky/vim-cuesheet) (cuesheet filetype)
- [dart](https://github.com/dart-lang/dart-vim-plugin) (dart filetype)
- [dhall](https://github.com/vmchale/dhall-vim) (dhall filetype)
- [dlang](https://github.com/JesseKPhillips/d.vim) (d, dcov, dd, ddoc, dsd and dsdl filetypes)
- [dockerfile](https://github.com/ekalinin/Dockerfile.vim) (yaml.docker-compose filetype)
- [elixir](https://github.com/elixir-lang/vim-elixir) (elixir, eelixi and eelixir filetypes)
- [elm](https://github.com/andys8/vim-elm-syntax) (elm filetype)
- [emberscript](https://github.com/yalesov/vim-ember-script) (ember-script filetype)
- [emblem](https://github.com/yalesov/vim-emblem) (emblem filetype)
- [erlang](https://github.com/vim-erlang/vim-erlang-runtime) (erlang filetype)
- [fennel](https://github.com/bakpakin/fennel.vim) (fennel filetype)
- [ferm](https://github.com/vim-scripts/ferm.vim) (ferm filetype)
- [fish](https://github.com/georgewitteman/vim-fish) (fish filetype)
- [flatbuffers](https://github.com/dcharbon/vim-flatbuffers) (fbs filetype)
- [fsharp](https://github.com/ionide/Ionide-vim) (fsharp filetype)
- [gdscript](https://github.com/calviken/vim-gdscript3) (gdscript3 filetype)
- [git](https://github.com/tpope/vim-git) (gitconfig, gitrebase, gitsendemail, gitcommi and gitcommit filetypes)
- [gitignore](https://github.com/fszymanski/fzf-gitignore) (gitignore filetype)
- [glsl](https://github.com/tikhomirov/vim-glsl) (glsl filetype)
- [gmpl](https://github.com/maelvalais/gmpl.vim) (gmpl filetype)
- [gnuplot](https://github.com/vim-scripts/gnuplot-syntax-highlighting) (gnuplot filetype)
- [go](https://github.com/fatih/vim-go) (go, gomod, gohtmltmp and gohtmltmpl filetypes)
- [gradle](https://github.com/tfnico/vim-gradle)
- [graphql](https://github.com/jparise/vim-graphql) (graphql filetype)
- [haml](https://github.com/tpope/vim-haml) (haml filetype)
- [handlebars](https://github.com/mustache/vim-mustache-handlebars) (html.mustache, html.handlebar and html.handlebars filetypes)
- [haproxy](https://github.com/CH-DanReif/haproxy.vim) (haproxy filetype)
- [haskell](https://github.com/neovimhaskell/haskell-vim) (haskell filetype)
- [haxe](https://github.com/yaymukund/vim-haxe) (haxe filetype)
- [hcl](https://github.com/b4b4r07/vim-hcl) (hcl filetype)
- [helm](https://github.com/towolf/vim-helm) (helm filetype)
- [help](https://github.com/neovim/neovim/tree/master/runtime) (help filetype)
- [hive](https://github.com/zebradil/hive.vim) (hive filetype)
- [html5](https://github.com/sheerun/html5.vim)
- [i3](https://github.com/mboughaba/i3config.vim) (i3config filetype)
- [icalendar](https://github.com/chutzpah/icalendar.vim) (icalendar filetype)
- [idris2](https://github.com/edwinb/idris2-vim) (idris2, lidris and lidris2 filetypes)
- [idris](https://github.com/idris-hackers/idris-vim) (idris filetype)
- [ion](https://github.com/vmchale/ion-vim) (ion filetype)
- [javascript-sql](https://github.com/statico/vim-javascript-sql)
- [javascript](https://github.com/pangloss/vim-javascript) (javascript, flo and flow filetypes)
- [jenkins](https://github.com/martinda/Jenkinsfile-vim-syntax) (Jenkinsfile filetype)
- [jq](https://github.com/vito-c/jq.vim) (jq filetype)
- [json5](https://github.com/GutenYe/json5.vim) (json5 filetype)
- [json](https://github.com/elzr/vim-json) (json filetype)
- [jsonnet](https://github.com/google/vim-jsonnet) (jsonnet filetype)
- [jst](https://github.com/briancollins/vim-jst) (jst filetype)
- [jsx](https://github.com/MaxMEllon/vim-jsx-pretty) (javascriptreact filetype)
- [julia](https://github.com/JuliaEditorSupport/julia-vim) (julia filetype)
- [kotlin](https://github.com/udalov/kotlin-vim) (kotlin filetype)
- [ledger](https://github.com/ledger/vim-ledger) (ledger filetype)
- [lilypond](https://github.com/anowlcalledjosh/vim-lilypond) (lilypond filetype)
- [livescript](https://github.com/gkz/vim-ls) (livescript filetype)
- [llvm](https://github.com/rhysd/vim-llvm) (llvm, tablege and tablegen filetypes)
- [log](https://github.com/MTDL9/vim-log-highlighting) (log filetype)
- [lua](https://github.com/tbastos/vim-lua) (lua filetype)
- [mako](https://github.com/sophacles/vim-bundle-mako) (mako filetype)
- [markdown](https://github.com/plasticboy/vim-markdown) (markdown filetype)
- [mathematica](https://github.com/voldikss/vim-mma) (mma filetype)
- [mdx](https://github.com/jxnblk/vim-mdx-js) (markdown.mdx filetype)
- [meson](https://github.com/mesonbuild/meson/tree/master/data/syntax-highlighting/vim) (meson, dosin and dosini filetypes)
- [moonscript](https://github.com/leafo/moonscript-vim) (moon filetype)
- [nginx](https://github.com/chr4/nginx.vim) (nginx filetype)
- [nim](https://github.com/zah/nim.vim) (nim filetype)
- [nix](https://github.com/LnL7/vim-nix) (nix filetype)
- [objc](https://github.com/b4winckler/vim-objc) (objc filetype)
- [ocaml](https://github.com/rgrinberg/vim-ocaml) (ocaml, omake, opam, oasis, dune, ocamlbuild_tags, ocpbuild, ocpbuildroot, sexpli and sexplib filetypes)
- [octave](https://github.com/McSinyx/vim-octave) (octave filetype)
- [odin](https://github.com/Tetralux/odin.vim) (odin filetype)
- [opencl](https://github.com/petRUShka/vim-opencl) (opencl filetype)
- [perl](https://github.com/vim-perl/vim-perl) (perl, pod, mason, tt2, tt2html, x and xs filetypes)
- [pgsql](https://github.com/lifepillar/pgsql.vim) (sql filetype)
- [php](https://github.com/StanAngeloff/php.vim) (php filetype)
- [plantuml](https://github.com/aklt/plantuml-syntax) (plantuml filetype)
- [pony](https://github.com/jakwings/vim-pony) (pony filetype)
- [powershell](https://github.com/PProvost/vim-ps1) (ps1, ps1xm and ps1xml filetypes)
- [protobuf](https://github.com/uarun/vim-protobuf) (proto filetype)
- [pug](https://github.com/digitaltoad/vim-pug) (pug filetype)
- [puppet](https://github.com/rodjek/vim-puppet) (puppet, embeddedpuppe and embeddedpuppet filetypes)
- [purescript](https://github.com/purescript-contrib/purescript-vim) (purescript filetype)
- [python-compiler](https://github.com/aliev/vim-compiler-python)
- [python-indent](https://github.com/Vimjas/vim-python-pep8-indent)
- [python](https://github.com/vim-python/python-syntax) (python filetype)
- [qmake](https://github.com/artoj/qmake-syntax-vim) (qmake filetype)
- [qml](https://github.com/peterhoeg/vim-qml) (qml filetype)
- [r-lang](https://github.com/vim-scripts/R.vim) (r, rhel and rhelp filetypes)
- [racket](https://github.com/wlangstroth/vim-racket) (racket filetype)
- [ragel](https://github.com/jneen/ragel.vim) (ragel filetype)
- [raku](https://github.com/Raku/vim-raku) (raku filetype)
- [raml](https://github.com/IN3D/vim-raml) (raml filetype)
- [razor](https://github.com/adamclerk/vim-razor) (razor filetype)
- [reason](https://github.com/reasonml-editor/vim-reason-plus) (reason filetype)
- [requirements](https://github.com/raimon49/requirements.txt.vim) (requirements filetype)
- [rspec](https://github.com/keith/rspec.vim) (ruby filetype)
- [rst](https://github.com/marshallward/vim-restructuredtext) (rst filetype)
- [ruby](https://github.com/vim-ruby/vim-ruby) (ruby, erub and eruby filetypes)
- [rust](https://github.com/rust-lang/rust.vim) (rust filetype)
- [scala](https://github.com/derekwyatt/vim-scala) (scala filetype)
- [scss](https://github.com/cakebaker/scss-syntax.vim) (scss filetype)
- [sh](https://github.com/arzg/vim-sh) (sh, zs and zsh filetypes)
- [slim](https://github.com/slim-template/vim-slim) (slim filetype)
- [slime](https://github.com/slime-lang/vim-slime-syntax) (slime filetype)
- [smt2](https://github.com/bohlender/vim-smt2) (smt2 filetype)
- [solidity](https://github.com/tomlion/vim-solidity) (solidity filetype)
- [stylus](https://github.com/wavded/vim-stylus) (stylus filetype)
- [svelte](https://github.com/evanleck/vim-svelte/tree/main) (svelte filetype)
- [svg-indent](https://github.com/jasonshell/vim-svg-indent)
- [svg](https://github.com/vim-scripts/svg.vim) (svg filetype)
- [swift](https://github.com/keith/swift.vim) (swift filetype)
- [sxhkd](https://github.com/baskerville/vim-sxhkdrc) (sxhkdrc filetype)
- [systemd](https://github.com/wgwoods/vim-systemd-syntax) (systemd filetype)
- [textile](https://github.com/timcharper/textile.vim) (textile filetype)
- [thrift](https://github.com/solarnz/thrift.vim) (thrift filetype)
- [tmux](https://github.com/ericpruitt/tmux.vim/tree/master/vim) (tmux filetype)
- [toml](https://github.com/cespare/vim-toml) (toml filetype)
- [tptp](https://github.com/c-cube/vim-tptp) (tptp filetype)
- [twig](https://github.com/lumiliet/vim-twig) (html.twig, xml.twi and xml.twig filetypes)
- [typescript](https://github.com/HerringtonDarkholme/yats.vim) (typescript, typescriptreac and typescriptreact filetypes)
- [unison](https://github.com/unisonweb/unison/tree/trunk/editor-support/vim) (unison filetype)
- [v](https://github.com/ollykel/v-vim) (vlang filetype)
- [vala](https://github.com/arrufat/vala.vim) (vala filetype)
- [vbnet](https://github.com/vim-scripts/vbnet.vim) (vbnet filetype)
- [vcl](https://github.com/smerrill/vcl-vim-plugin) (vcl filetype)
- [velocity](https://github.com/lepture/vim-velocity) (velocity filetype)
- [vue](https://github.com/posva/vim-vue) (vue filetype)
- [xdc](https://github.com/amal-khailtash/vim-xdc-syntax) (xdc filetype)
- [xml](https://github.com/amadeus/vim-xml) (xml filetype)
- [xsl](https://github.com/vim-scripts/XSLT-syntax) (xsl filetype)
- [yard](https://github.com/noprompt/vim-yardoc)
- [zephir](https://github.com/xwsoul/vim-zephir) (zephir filetype)
- [zig](https://github.com/ziglang/zig.vim) (zir, zi and zig filetypes)
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
