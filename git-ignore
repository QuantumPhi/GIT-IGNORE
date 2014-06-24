#!/bin/bash

if [[ -z "$1" ]]
then
    printf "\nGit Ignore\n\n"
    printf "Usage:\n"
    printf "    git ignore [OPTIONS]\n\n"
    printf "Options:\n"
    printf "    list - List available templates\n"
    printf "    <TEMPLATE> - Create .gitignore template\n"
    printf "    <FILE> - Ignore local file\n\n"
elif [[ "$1" == "list" ]]
then
    gitignorer $1
elif [[ -e "$(pwd)/$1" || -d "$(pwd)/$1" ]]
then
    echo -e "$1" >> .gitignore
    sort .gitignore -o .gitignore
elif [[ ! -z "'$(gitignorer list)' | grep -Fx '$1' > /dev/null" ]]
then
    gitignorer create $1
fi
