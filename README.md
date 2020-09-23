<div align="center">

## Convert UPPERCASE STRING to lower case string


</div>

### Description

Just what the title says. Convert Upper to lower case.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Josh Nixon](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/josh-nixon.md)
**Level**          |Beginner
**User Rating**    |4.0 (12 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/josh-nixon-convert-uppercase-string-to-lower-case-string__3-4114/archive/master.zip)

### API Declarations

iostream.h


### Source Code

```
void STRING::StrLwr(char* mainstring, char *output)
 {
 int Len = strlen(mainstring), Index;
 for(int i = 0; i < Len; i++)
  {
  if( (int)mainstring[i] < 65)
  output[i] = mainstring[i];
  if( (int)mainstring[i] >= 65 && (int)mainstring[i] <= 90)
  output[i] = (char)mainstring[i] + 32;
  if( (int)mainstring[i] >= 97 && (int)mainstring[i] <= 122)
  output[i] = (char)mainstring[i];
  if( (int)mainstring[i] > 122)
  output[i] = mainstring[i];
  Index++;
  }
  output[Index] = 0;
 }
```

