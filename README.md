# ejs-get-started

Getting started with ejs.（ejs 使用示例）

**Install**

```sh
$ pnpm add ejs
$ pnpm add @types/ejs -D
```

**Example**

```ts
import { Textarea } from 'ant-design-vue';
import ejs from 'ejs';

const a = `<% if(name) { -%>
  Hello, <%= name %>
<% } %>`;
let b = '';

b = ejs.render(a, { name: 'EJS' });
```



## <%= ... %>

template:
```txt
Hello, <%= name %>!
```

rendered: 
```
Hello, EJS!
```



## <%- ... %>

template:
```txt
<%= name %>
<%- name %>
```

rendered:
```txt
&lt;strong&gt;Hello, World!&lt;/strong&gt;
<strong>Hello, World!</strong>
```



## <% ... %>

template:
```txt
<% if(name) { %>
Hello, <%= name %>
<% } %>
```

rendered:
```txt

Hello, EJS
```



## <%_ ... %>

template:
```txt
     <%_ %>Hello, <%= name %>!
```

rendered:
```txt
Hello, EJS!
```



## <% ... _%>

template:
```txt
Hello, <%= text _%>          !
```

rendered:
```txt
Hello, EJS!
```



## <%# ... %>

template:
```txt
<%# This is a comment %>
<%= text %>
```

rendered:
```txt

Hello, World!
```



## <%% ... %%>

template:
```txt
<%= text %>
<%%= text %%>
```

rendered:
```txt
Hello, World!
<%= text %>
```



## <% ... -%>

template:
```txt
<%# This is a comment -%>
<%= text %>
```

rendered:
```txt
Hello, World!
```
