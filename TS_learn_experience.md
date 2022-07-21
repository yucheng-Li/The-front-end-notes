### 怎么将JS模块引入TS ？
https://bobbyhadz.com/blog/typescript-could-not-find-a-declaration-file-for-module
+   1. 直接安装模块对应的类型注解文件（前提是得有） npm i --save-dev @types/uuid
+   2. 同目录下 .d.ts
+   3.  加入忽略ts检查的提醒
        ```js
            // eslint-disable-next-line @typescript-eslint/ban-ts-comment
            // @ts-ignore
            import { myFunction } from 'module-name';
        ```
### Variable 'X' is used before being assigned in TypeScript
https://bobbyhadz.com/blog/typescript-variable-is-used-before-being-assigned
+   需要给定义的变量一个初始值

### Element implicitly has an 'any' type because expression of type 'string' can't be used to index type
https://bobbyhadz.com/blog/typescript-element-implicitly-has-any-type-expression
+   实际上是使用了类型断言告诉了typescript一定会存在该key