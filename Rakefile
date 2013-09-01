require 'sinatra/activerecord/rake'
require './app'

desc "This task is called by the Heroku Scheduler add-on: rake sync:github"

task :app do
  require './app'
end

LANGUAGES = %w(ABAP
               ActionScript
               Ada
               Apex
               AppleScript
               Arc
               Arduino
               ASP
               Assembly
               Augeas
               AutoHotkey
               Awk
               Boo
               Bro
               C
               C%23
               C++
               Ceylon
               CLIPS
               Clojure
               CoffeeScript
               ColdFusion
               Common%20Lisp
               Coq
               D
               Dart
               DCPU-16%20ASM
               Delphi
               DOT
               Dylan
               eC
               Ecl
               Eiffel
               Elixir
               Emacs%20Lisp
               Erlang
               F%23
               Factor
               Fancy
               Fantom
               Forth
               FORTRAN
               Go
               Gosu
               Groovy
               Haskell
               Haxe
               Io
               Ioke
               Java
               JavaScript
               Julia
               Kotlin
               Lasso
               LiveScript
               Logos
               Logtalk
               Lua
               M
               Matlab
               Max
               Mirah
               Monkey
               MoonScript
               Nemerle
               Nimrod
               Nu
               Objective-C
               Objective-J
               OCaml
               Omgrofl
               ooc
               Opa
               OpenEdge%20ABL
               Parrot
               Perl
               PHP
               Pike
               PogoScript
               PowerShell
               Processing
               Prolog
               Puppet
               Pure%20Data
               Python
               R
               Racket
               Ragel%20in%20Ruby%20Host
               Rebol
               Rouge
               Ruby
               Rust
               Scala
               Scheme
               Scilab
               Self
               Shell
               Slash
               Smalltalk
               Standard%20ML
               SuperCollider
               Tcl
               Turing
               TXL
               TypeScript
               Vala
               Verilog
               VHDL
               VimL
               Visual%20Basic
               wisp
               XC
               XML
               XProc
               XQuery
               XSLT
               Xtend
               ).freeze

namespace :sync do
  task :github => :app do
    Leaderboard.fetch(LANGUAGES)
  end
end