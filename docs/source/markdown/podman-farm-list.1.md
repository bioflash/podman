% podman-farm-list 1

## NAME
podman\-farm\-list - List the existing farms

## SYNOPSIS
**podman farm list** [*options*]

**podman farm ls** [*options*]

## DESCRIPTION
List all the existing farms.

## OPTIONS

#### **--format**, **-f**=*format*

Change the default output format.  This can be of a supported type like 'json' or a Go template.
Valid placeholders for the Go template listed below:

| **Placeholder** | **Description**                            |
| --------------- | ------------------------------------------ |
| .Connections    | List of all system connections in the farm |
| .Default        | Indicates whether farm is the default      |
| .Name           | Farm name                                  |

## EXAMPLE
```
$ podman farm list
Name        Connections  Default
farm1       [f38 f37]    false
farm2       [f37]        true
```
## SEE ALSO
**[podman(1)](podman.1.md)**, **[podman-farm(1)](podman-farm.1.md)**

## HISTORY
July 2023, Originally compiled by Urvashi Mohnani (umohnani at redhat dot com)
