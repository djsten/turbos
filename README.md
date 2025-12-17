# TurbOS

# VERSION INDICATIONS
evil: like really buggy or unfinished
÷: prerelease

# COMMANDS

ignore ()*[]

get (*tv *var) link

floatv var

brc message

localfile loadtovar var

output show/hide

varset name value

sh_util (imp (spr v var) (ext link))

rxfs (ls file) (set filename data) (export)

bg bg-name

clr

clip tv var-name 

reset

strue var-name

update (dcb)

install (dcb)


# DCB INSTRUCTIONS

# Variables:

DCB_restart: Restarts the lists, inputs, and sprite

DCB_run: use "strue" as it is a broadcast with no broadcast option

DCB_input: the input, use clipboard or file for this

# Options:

# [KEY]

[] -> Note
() -> Usage
-> -> Meaning
{} -> For multi meanings, do not include instead refer to usage ()

global% -> changes a local storage key (global% "keyname" "value")

print -> prints to the dcb output (print "input")

hideoutput -> hides the output (standalone)

showoutput -> shows the output (standalone)

import {

  sprite -> imports a sprite (import sprite dataURI)
  
  extension -> imports an extension (import extension url)
  
}

$list - a list [cant do anything yet] {

  add -> adds a string to the list ($list add "string input")

  setarray -> currently broken in v1 but sets the list to a json array ($list setarray "array string")
  
}

stamp -> stamps a sprite (stamp spritename)

erase -> erase all from pen extansion (standalone)

wait -> delays the script (wait int)

