
Run `yarn dev`. This will build and serve both `application-a` and `application-b` on ports 3001 and 3002 respectively.

配置属性：

   name，必须，唯一 ID，作为输出的模块名，使用的时通过 ${name}/${expose} 的方式使用；

   library，必须，其中这里的 name 为作为 umd 的 name；

   remotes，可选，表示作为 Host 时，去消费哪些 Remote；

   exposes，可选，表示作为 Remote 时，export 哪些属性被消费；

   shared，可选，优先用 Host 的依赖，如果 Host 没有，再用自己的；