---
title: "TypeScript入门教程(十四) - 装饰器"
date: 2018-10-22 21:00
tags:
 - TypeScript
---

随着`TypeScript`和`ES6`里引入了类，在一些场景下我们需要额外的特性来支持标注或修改类及其成员。 装饰器（`Decorators`）为我们在类的声明及成员上通过元编程语法添加标注提供了一种方式。 `Javascript`里的装饰器目前处在`建议征集的第二阶段`，但在`TypeScript`里已做为一项实验性特性予以支持

<!--more-->

### 介绍

若要启用实验性的装饰器特性，你必须在命令行或`tsconfig.json`里启用`experimentalDecorators`编译器选项

* 命令行:
```typescript
tsc --target ES5 --experimentalDecorators
```
* tsconfig.json:
```json
{
    "compilerOptions": {
        "target": "ES5",
        "experimentalDecorators": true
    }
}
```

### 装饰器

