# vuets-order

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### What have I learned

* 5-1.`<a href="/menu"></a>`Ҳ������ת·�ɣ����ǻ��С�ˢ�¡�������Ҫ�滻��`<router-link to="/menu">�˵�</router-link>`
* 5-2.navbar����ĵ�¼��ע���ulӦ����`ml-auto`
* 5-3.router-link���������`to="/menu"===to="menu"`
* 6-1.router-link��`tag`����
* 6-2.router-link����to�Ķ�̬��`:to="variable-name"`
* 6-3.������router���ڣ���д��`{path: '*',redirect: '/',}`
* 7-1.·������name���ԣ����õ�ʱ����`:to="{name: homeLink}"`
* 7-2.·����ת��ʽ��
```javascript
changeRouter () {
    //
    this.$router.��go��(-1);
    //
    this.$router.��replace��('/menu');
    this.$router.replace({name: 'menuLink'});
    //
    this.$router.��push��('/menu');
    this.$router.push({name: 'menuLink'});
}
```
* 8-1.����·�ɺ�����·��
```javascript
һ��redirect: '/admin',
����redirect: '/admin/contact'
����redirect: '/admin/contact/phone'
```
*9-1.ȫ������
```javascript
router.beforeEach((to, from, next) => {
	if (to.path === '/login' || to.path === '/register') {
        next();
    } else {
        if (!true) {
            next();
        } else {
            next('/login');
        }
    }
})
```
9-2.
���ù���
```javascript
router.afterEach((to, from) => {

})
```
��������
```javascript
router.beforeEnter((to, from, next) => {
    
})
```























