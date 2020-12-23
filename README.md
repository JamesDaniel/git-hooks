#!/bin/bash
#.git/hooks/commit-msg
MSG=`cat $1`

if [[ "$MSG" =~ ^Merged.* ]]; then
    exit 0
fi

if ! [[ $MSG =~ ^DP-[0-9]{1,}.* ]]; then
    echo "Error: "
    echo "    "Commit message must reference a Jira number. E.g. DP-1234
    exit 1
fi


# https://github.com/typicode/husky/tree/master
