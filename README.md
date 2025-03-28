**code-audit** is a [Nerve](https://github.com/evilsocket/nerve) agent that performs a security audit on a target codebase and saves its findings to `AUDIT.md` in markdown.

Install with (requires nerve >= 1.4.x):

```bash
# this will download and install (or update) to ~/.nerve/agents
nerve install evilsocket/code-audit 
```

By default it will scan the current folder:

```bash
nerve run code-audit
```

To specify another path use the `--target-path` argument:

```bash
nerve run code-audit --target-path /path/to/code
```

The security audit findings will be automatically appended to the `AUDIT.md` file in the current working directory for easy review and documentation.