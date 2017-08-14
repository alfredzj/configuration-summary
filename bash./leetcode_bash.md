# Bash

### 1. ```grep``` ```sed``` ```awk```
```grep```: print lines matching a pattern  
``` grep [OPTIONS] PATTERN [FILE...]```   
``` grep [OPTIONS] [-e PATTERN]... [-f FILE]... [FILE...]```

```sed```: stream editor for filtering and transforming text  
```sed [OPTION]... {script-only-if-no-other-script} [INPUT_FILE]```

```awk```: pattern scanning and text processing language        
```mawk  [-W  option]  [-F value] [-v var=value] [--] 'program text' [file...]```   
```mawk [-W option] [-F value] [-v var=value] [-f program-file] [--] [file...]```

##### Regular Expression
- Boolean "or"    
   A vertical bar separates alternatives. For example, gray|grey can match "gray" or "grey".
- Grouping    
   Parentheses are used to define the scope and precedence of the operators (among other uses). For example, gray|grey and gr(a|e)y are equivalent patterns which both describe the set of "gray" or "grey".

https://leetcode.com/problems/valid-phone-numbers/description/
