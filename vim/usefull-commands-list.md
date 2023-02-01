# Motion commands
]'

['

m{a-zA-Z}
Set mark {a-zA-Z} at cursor position.

:g :global
:[range]g[lobal]/{pattern}/[cmd]
Execute the Ex command [cmd] (default ":p") on the lines within [range] where {pattern} matches.

:h ex-cmd-index
show ex commands that can be used in global
