---
title: "docker-compose.yml tab error"
description: "docker-compose.yml에 tab을 넣으면 에러가 발생한다. tab을 없애 에러를 해결한다."
---

다음과 같은 에러가 발생했다:

```
ERROR: yaml.scanner.ScannerError: while scanning for the next token
found character '\t' that cannot start any token
  in "./docker-compose.yml", line 14, column 1
```

해당 라인에 tab(\t)이 있어서 나는 에러이다. 해당 라인에 있는 tab을 space로 변경하면 에러가 해결된다.
