# react-admin

> React 17+React-Router4 从零打造企业级电商后台管理系统

## 后端接口
- login
 ```js
  {
    ret: '0',
    msg: '成功',
    data: {
      permissions: [
        'login',
        ...
      ],
      role: '系统管理员',
      roleType: 1,   // 1 管理员 2 运营人员 0 游客，
      uid: 1,
      userName: '系统管理员',
      avatar: ''
    }
  }
 ```
- menus

```js
// roleType = 1
{
  ret: '0',
  msg: '成功',
  menus: [
    {
      component: '表格',
      path: '/table',
      key: '/table',
      sub: [{
          component: '基本表格',
          path: '/table/basicTable',
          key: '/table/basicTable'
        },
        {
          component: '高级表格',
          path: '/table/advancedTable',
          key: '/table/advancedTable'
        },
        {
          component: '异步表格',
          path: '/table/asynchronousTable',
          key: '/table/asynchronousTable'
        },
      ]
    }
  ]
}
```
