# UML Class Diagram

| **Class**   |
|--------|
| -privateMember: int   |
| #protectedMember: char  |
| +publicMember: bool |
|──────────────────────────|
| +publicMethod(): void  |
| +_publicVirtualMethod(parameter: int): void_  |
| -privateMethod(): bool |
| #protectedMethod(value: int): char |

**Generalization**
```python
|       Child Class      |      is a      |       Parent Class       |
|       -kid: bool       |  ───────────▷  |  +virtualMethod(): void  |
| +virtualMethod(): void |
```

**Realization**
```python
|         Class          |   Implements   |         Interface        |
|       -kid: bool       |  - - - - - -▷  |  +virtualMethod(): void  |
| +virtualMethod(): void |
```

**Association**
```python
          1..*             1
| Class 1 |  ───────────▶  | Class 2|

```

**Dependency**
```python
               <<use>>
| Class 1 |  - - - - - ->  | Class 2|

```

**Aggregation**
```python
          1    <<has a>>   1..*
| Class 1 |  ◇───────────  | Class 2|

```

**Composition**
```python
          1   <<owns a>>   1..*
| Class 1 |  ◆───────────  | Class 2|

```
