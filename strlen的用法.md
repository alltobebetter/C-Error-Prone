# strlen的用法

**需要引入的头文件：**

```c
#include <string.h>
```

**调用 `strlen`**：

你可以将一个字符串传递给 `strlen` 函数，它将返回该字符串的长度（以字符为单位，不包含\0）。

**示例代码**

```c
#include <stdio.h>
#include <string.h>

int main() {
    const char *str = "Hello, World!";
    size_t length = strlen(str); // 获取字符串长度

    printf("字符串长度: %zu\n", length); // 输出长度
    return 0;
}
```

**注意事项**

- `strlen` 返回值类型是 `size_t`，它是一个无符号整数类型，通常用于表示对象的大小。
- 确保传递给 `strlen` 的字符串是以 `\0` 结尾的，否则可能导致未定义行为。
- `strlen` 计算的是字符的数量，不包括结束符 `\0`。
