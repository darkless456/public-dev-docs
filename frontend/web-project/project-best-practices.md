# Front Project

## 简单查询列表展示页

可以使用统一模板：[simple-query-page](./simple-query-page.md)

## Suggestion

- 简单查询条件 `form` 统一使用 `shf-item` 组件，较复杂（需要我们自己控制布局 长短的）统一使用 `nz row + nz col`

- `spin` 统一使用 `BehaviorSubject`, 定义一个 `showSpin/hideSpin` 方法， 如果需要改变 `nzTip` 则 `showSpin(nzTip)`

- `Component` 中 方法名可以简单 `query add update delete` ，但是必须有注释

- `Http Service` 中方法名参照 Api 命名， 且必须有注释。命名风格 `const getXxxApi = admin/xxx/getXxx`

- 统一使用 `Router Service` 进行页面跳转，并且保证 一个 module 一个 router

- `Simple table`, 显示金额时，统一加上: `type: 'currency'`
