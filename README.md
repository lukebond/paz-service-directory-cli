paz-service-directory-cli
=========================

CLI for the paz service directory.

## Usage

```
Usage:
  paz-svcdir-cli [OPTIONS] <command> [ARGS]

Options:
  -h, --host [HOST]      paz service-directory server hostname (Default is localhost)
  -p, --port [NUMBER]    paz service-directory server port (Default is 9000)
  -j, --json BOOLEAN     Produce JSON output
  -f, --file BOOLEAN     Outputs unitfile to a file instead of stdout (uses
                         <service name>.service)
  -s, --set STRING       Sets field values. Only applies to 'modify' command,
                         for which it is required. Either pass @filename or
                         send comma-delimited key-value pairs (e.g. --set
                         key=value,key=value...). Only the following
                         fields are settable via the latter method: name,
                         dockerImage, gitReceiveHook, autoDeploy,
                         numInstances.
  -q, --quiet BOOLEAN    Suppress table header in output.
  -i, --index [NUMBER]   Index of the unit file to output (0-based). (Default is -1)

Commands:
  delete, list, modify, show, unitfile
```
