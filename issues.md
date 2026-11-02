
# Static Code Analysis – Issues and Fixes

| Issue | Tool | Type | Description | Fix |
|---|---|---|---|---|
| Mutable default argument | Pylint | Bug | players=[] was shared between function calls | Changed default to None |
| Poor function naming | Pylint | Code quality | Functions used camelCase | Converted to snake_case |
| Missing docstrings | Pylint | Code quality | Functions lacked documentation | Added docstrings |
| Hardcoded password | Bandit | Security | Referee password was stored in source code | Removed hardcoded credential |
| Insecure temporary file | Bandit | Security | tempfile.mktemp() was unsafe | Used NamedTemporaryFile |
| Unsafe shell execution | Bandit | Security | os.system() could allow command injection | Used subprocess with argument list |
| Whitespace before colon | Flake8 | Style | Incorrect spacing | Corrected spacing |
| Missing blank lines | Flake8 | Style | Insufficient blank lines | Added blank lines |
| Missing whitespace | Flake8 | Style | Missing whitespace after punctuation | Corrected spacing |
| Inline comment spacing | Flake8 | Style | Incorrect comment spacing | Corrected formatting |

## Conclusion

Static code analysis helped identify programming mistakes, security vulnerabilities and style violations. Pylint improved code quality, Bandit helped identify security risks, and Flake8 improved formatting and readability.
