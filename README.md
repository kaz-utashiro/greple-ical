# NAME

ical - Module to support Apple OS X Calendar data

# SYNOPSIS

greple -Mical \[ options \]

    --simple  print data in on line
    --detail  print one line data with descrition if available

Exported functions

    &print_ical_simple
    &print_ical_desc
    &print_ical_detail

# SAMPLES

greple -Mical ...

greple -Mical --simple ...

greple -Mical --detail ...

greple -Mical --all --print print\_desc ...

# DESCRIPTION

Used without options, it will search all OS X Calendar files under
user's home directory.

With **--simple** option, summarize content in single line.
Output is not sorted.

With **--detail** option, pirnt summrized line with description data if
it is attached.  The result is sorted.

Sample:

     BEGIN:VEVENT
     UID:19970901T130000Z-123401@host.com
     DTSTAMP:19970901T1300Z
     DTSTART:19970903T163000Z
     DTEND:19970903T190000Z
     SUMMARY:Annual Employee Review
     CLASS:PRIVATE
     CATEGORIES:BUSINESS,HUMAN RESOURCES
     END:VEVENT

# SEE ALSO

RFC2445

# AUTHOR

Kazumasa Utashiro

# LICENSE

Copyright 2017-2021 Kazumasa Utashiro.

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.