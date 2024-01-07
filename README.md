# UNRL
Eliminating duplicates of url with same parameter from stdin.

## Usage
```
> cat url.txt
https://example.com/test?a=aaaa&b=bbbbb
https://example.com/test?a=cccc&b=ddddd
https://example.com/test?a=zzzz&b=xxxxx
https://example.com/diff?a=aaaa&b=bbbbb
https://example.com/diff?a=aaaa&b=ddddd
```
Use ```unrl``` from stdin :
```
> cat url.txt | unrl

https://example.com/diff?a=&b=
https://example.com/test?a=&b=
```
