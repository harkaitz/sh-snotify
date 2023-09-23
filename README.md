# SNOTIFY

Simple script to use the [ntfy.sh](https://ntfy.sh) service with
servers. It uses wget. Supports busybox (even on windows).

## Help

snotify

    Usage: snotify [-V][-t TOPIC] [- | COMMAND...]
    
    Send notifications through "ntfy.sh".
    
      -V            : Show configuration files.
      -c            : Perform check.
      -m MESSAGE    : Specify message from command line.
      -H            : High priority.
      -T TITLE      : Pack as code.
      -t TOPIC      : Topic to send to, NTFY_TOPIC_PREFIX is set
                      then ${NTFY_TOPIC_PREFIX}--TOPIC will be used.
      -E TOPIC      : Topic to send to, ignore NTFY_TOPIC_PREFIX.
    
    Environment   : NTFY_TOPIC_PREFIX
    Files UNIX    : ~/.snotify, /etc/snotify
    Files WINDOWS : ~/.snotify, $winsysdir/snotify.txt

snotify-install

    Usage: snotify-install [ssh MACHINE]
    
    Install snotify in [a remote] system with the same configuration.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
