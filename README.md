# Notable Mentions
I would like to acknowledge the following books that have greatly influenced my understanding of design patterns and software development:
- Mastering Design Patterns by Ta Van Dung ([Book Repo](https://github.com/tvd12/master-design-patterns), [tvd12](https://tvd12.com/design-pattern/))
- Design Patterns: Elements of Reusable Object-Oriented Software by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides (Gang of Four)
- Dive Into Design Patterns by Alexander Shvets ([refactoring.guru](https://refactoring.guru/))
- Clean Code: A Handbook of Agile Software Craftsmanship by Robert C. Martin

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
| Class 1 |  ───────────▶  | Class 2 |

```

**Dependency**
```python
               <<uses>>
| Class 1 |  - - - - - ->  | Class 2 |

```

**Aggregation**
```python
          1    <<has a>>   1..*
| Class 1 |  ◇───────────  | Class 2 |

```

**Composition**
```python
          1   <<owns a>>   1..*
| Class 1 |  ◆───────────  | Class 2 |

```
