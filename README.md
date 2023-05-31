# Command_Injection

## Detecting Command Injection
| Injection Method| Injection Character| URL-Encoded Character| Executed Command|
|---|---|---|---|
|Semicolon|;|%3b|Both
|New line|\n|%0a|Both
|Background|&|%26|Both (second output shown first)
|Pipe|\||%7c|Both (only second output is shown)
|AND|&&|%26%26|Both (Only if first Succeeds)
|OR|\|\||%7c%7c|Second (only if first fails)
|Sub-Shell|\`\`|%60%60|Both (Linux-only)
|Sub-Shell|$()|%24%28%29|Both (Linux-only)
