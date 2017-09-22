---
layout: post
title: "Timezones with Jekyll"
author: "Andrew Lazarus"
date: 2015-11-01 12:44:24 +0100
tags:
- timezones
- jekyll
- development
meta:
 svg_header: '<svg xmlns="http://www.w3.org/2000/svg" width="246.3" height="151.3" viewBox="0 0 246.3 151.3"><style>.st0{fill:#010101;} .st1{fill:#ED1F24;}</style><path id="XMLID_72_" class="st0" d="M82.2 10.6c-3.3-2.5-8-5-13-6.9C63 1.3 57.2 0 52.8 0c-5.6 0-7.8 2.3-8.5 4.3 0 .1-.1.2-.1.3l-.2.3c-.2.8-.2 1.6-.1 2.5.4 2.9.4 5.7.1 6.4L1.4 124.5 0 128.1l.4.2c-1.4 9.1 3.7 18.4 12.5 21.7 2.3.9 4.7 1.3 7.1 1.3 6.7 0 12.8-3.3 16.6-8.7l.5.2L81.2 28.1c.3-.7 2.2-2.8 4.4-4.7.7-.5 1.2-1.2 1.5-1.9l.3-.6c1.2-3.3-.5-6.8-5.2-10.3zM14.9 144.8c-7.3-2.8-11-11.1-8.3-18.4l.1-.3L49.1 15.7c1.1-2.9.2-8.6.2-9.2v-.2c0-.3.9-.8 3.4-.8 3.7 0 9.1 1.2 14.5 3.3 4.6 1.8 8.7 4 11.6 6.1 3 2.3 3.4 3.6 3.3 3.9 0 0 0 .1-.1.1l-.1.1c-.9.8-5.1 4.6-6 7L33.5 136.3l-.2.4c-2.2 5.5-7.4 9.1-13.3 9.1-1.8-.1-3.5-.4-5.1-1z"/><path id="XMLID_62_" class="st1" d="M61.2 56s-5.9 6.8-11.2 9.2-9.3 1.8-14.1 4.6c-4.8 2.8-7.3 6.7-7.3 6.7L9 127.5c-2.1 5.8 1 12.5 6.9 14.7 5.8 2.3 12.4-.7 14.7-6.4L61.2 56zM41.5 85.4c.9-.4 2 0 2.4.9.4.9 0 2-.9 2.4-.9.4-2 0-2.4-.9-.5-.9 0-2 .9-2.4zM33.6 77c.6-.3 1.4 0 1.6.6s0 1.4-.6 1.6c-.6.3-1.4 0-1.6-.6-.3-.6 0-1.3.6-1.6zM25 105.9c-.9.4-2 0-2.4-.9-.4-.9 0-2 .9-2.4.9-.4 2 0 2.4.9.5.9.1 1.9-.9 2.4zm1.7-6.7c-.8-1.8 0-3.8 1.8-4.6 1.8-.8 3.8 0 4.6 1.8.8 1.8 0 3.8-1.8 4.6-1.8.7-3.8-.1-4.6-1.8zm4.5 17.6c.6-.3 1.4 0 1.6.6s0 1.4-.6 1.6c-.6.3-1.4 0-1.6-.6-.3-.5-.1-1.3.6-1.6z"/><ellipse id="XMLID_61_" transform="rotate(-68.96 65.214 13.748)" class="st0" cx="65.2" cy="13.7" rx="3.1" ry="11.8"/><g id="XMLID_40_"><g id="XMLID_57_"><path id="XMLID_58_" d="M108.6 73.5c.9 0 1.5.5 1.5 1.5v3.2c0 .9-.5 1.5-1.5 1.5h-8.1V88c0 .9-.5 1.5-1.5 1.5h-3.5c-.9 0-1.5-.5-1.5-1.5v-8.3h-8.1c-.9 0-1.5-.5-1.5-1.5V75c0-.9.5-1.5 1.5-1.5H94v-8.3c0-.9.5-1.5 1.5-1.5H99c.9 0 1.5.5 1.5 1.5v8.3h8.1z"/></g><g id="XMLID_52_"><path id="XMLID_53_" d="M147 77.1c0 14.6-6.5 21.2-15.8 21.2s-15.8-6.8-15.8-21.2c0-14.5 6.8-21.2 15.8-21.2 9.5 0 15.8 6.8 15.8 21.2zm-8.6 0c0-8-1.8-13.7-7.2-13.7-5.2 0-7.2 5.7-7.2 13.7 0 8.1 2.1 13.7 7.2 13.7 5.5 0 7.2-5.6 7.2-13.7z"/></g><g id="XMLID_49_"><path id="XMLID_50_" d="M167.2 56.5c.3-.2.8-.6 1.4-.6.9 0 1.3.6 1.3 1.6v38.8c0 .9-.5 1.5-1.5 1.5h-4.7c-.9 0-1.5-.5-1.5-1.5v-28l-6.8 4.8c-.3.2-.6.4-.9.4-.4 0-.8-.2-1.1-.7l-2.4-3.2c-.2-.3-.3-.6-.3-.9 0-.4.2-.8.6-1.1l15.9-11.1z"/></g><g id="XMLID_45_"><path id="XMLID_46_" d="M208.9 77.1c0 14.6-6.5 21.2-15.8 21.2s-15.8-6.8-15.8-21.2c0-14.5 6.8-21.2 15.8-21.2 9.5 0 15.8 6.8 15.8 21.2zm-8.6 0c0-8-1.8-13.7-7.2-13.7-5.2 0-7.2 5.7-7.2 13.7 0 8.1 2.1 13.7 7.2 13.7 5.4 0 7.2-5.6 7.2-13.7z"/></g><g id="XMLID_41_"><path id="XMLID_42_" d="M246.3 77.1c0 14.6-6.5 21.2-15.8 21.2s-15.8-6.8-15.8-21.2c0-14.5 6.8-21.2 15.8-21.2 9.6 0 15.8 6.8 15.8 21.2zm-8.5 0c0-8-1.8-13.7-7.2-13.7-5.2 0-7.2 5.7-7.2 13.7 0 8.1 2.1 13.7 7.2 13.7 5.4 0 7.2-5.6 7.2-13.7z"/></g></g></svg>'
author:
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus
    
---

Using Jekyll outside of jekyll's motherland? You're going to need to add your timezone to your date.

Here's a little script for you, save this as post.sh in your Jekyll root

    #!/bin/bash
    #---------/---------------------\---------#
    #--------|- Jekyll Post Creator -|--------#
    #---------\---------------------/---------#
    # Ripped and tweaked from https://gist.github.com/kabrooski/6107707
    
    # Simply put the script in your site directory, edit the configs to fit your setup, and run it with:
    # ./post "post title"
    
    # What is does:
    # - creates the post with the correct format of date and title
    # - adds YAML front-matter (layout, title, date, tags)
    # - opens the post file in editor chosen
    
    
    ########## Configs ##########
    
    # Post layout
    layout=post
    
    # Post text editor
    editor=Mou
    
    # Post directory
    folder=_posts/
    
    # Author
    author="Andrew Lazarus"
    
    ########## Program ##########
    
    # show help with -h
    if [ "$1" == "-h" ]; then
      echo "Usage: `basename $0` \"Post title\""
      exit 0
    elif [ -z "$1" ]; then
      echo "Usage: `basename $0` \"Post title\""
      exit 0
    fi
    
    # Y/n ask function
    function ask {
        while true; do
    
            if [ "${2:-}" = "true" ]; then
                prompt="Y/n"
                default=Y
            elif [ "${2:-}" = "false" ]; then
                prompt="y/N"
                default=N
            else
                prompt="y/n"
                default=
            fi
    
            # Ask the question
            read -p "$1 [$prompt] " REPLY
    
            # Default?
            if [ -z "$REPLY" ]; then
                REPLY=$default
            fi
    
            # Check if the reply is valid
            case "$REPLY" in
                Y*|y*) return 0 ;;
                N*|n*) return 1 ;;
            esac
    
        done
    }
    
    ##### Variables #####
    
    # post title
    title="$1"
    
    # convert title to filename format
    # echo part replaces spaces with '-'
    # awk converts it to lowercase
    # sed keeps only lowercase letters and '-'
    filetitle=$( echo ${1// /-} | awk '{print tolower($0)}'| sed 's/[^a-z\-]*//g')
    
    # name of file
    filename="$folder`date +%F`-$filetitle.md"
    echo $filename
    
    
    ########## Adding to file ##########
    echo "---" >> $filename
    echo "layout: $layout" >> $filename
    echo "title: \"$title\"" >> $filename
    echo "author: \"$author\"" >> $filename
    echo "date: `date +%F\ %H:%M:%S\ %z`" >> $filename
    
    
    ### Adding tags on new lines with a dash in front (separated with comma)
    read -p "Tags: " tags
    if [ "$tags" ]; then
      echo "tags:
    - $tags" | sed 's/,/\
    -/g' >> $filename
    fi
    
    echo "---" >> $filename
    echo >> $filename
    
    # open in chosen editor
    open -a $editor $filename

This should allow Jekyll to compile posts when you're out of the country.