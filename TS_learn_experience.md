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
    
