#后台管理系统

我写的第一个项目，完整的ts的封装的axios，因为当时项目不太熟悉，后端挂服务器上，使用了axios，并且baseurl使用的并非/api开头而是完整路径，
后端也是带有cors跨域的，所以没管，但是过段时间我的服务器因为我安装postgresql的时候装错了，可能装了点别的东西，给黑客留了个后门，所以
服务器改密码也没用，重置服务器的话我没有备份，而且我的博客项目的icon和小人和后端strapi都挂在服务器上，且服务器在23年的3月过期我就关了没管他了。  
所以里面的axios封装在当时没去改成/api，而是全部替换成了/api并使用useFetch请求，建议还是封装一下。axios的话后端是有跨域的但是后来不知道为什么又没了。所以把useFetch的地方换成axios把baseurl改成/api就可以了。

```bash
cd project-vue
pnpm i
pnpm dev
```

这是一个简易后台管理系统，后端开在云服务器上
如果需要使用api接口可以让我挂一下pm2，因为有timeout，因为后端不是我写的我不知道他放哪，我也懒得找

