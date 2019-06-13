# deploy_nodejs_app
## install pm2
PM2 is a production process manager for Node.js applications with a built-in load balancer. It allows you to keep applications alive forever, to reload them without downtime and to facilitate common system admin tasks.

```npm
npm install pm2 -g
```

### start an project
```npm
pm2 start app.js
```
### stop a project
```npm
pm2 stop app.js
```

## run it on port 80
```npm
sudo setcap cap_net_bind_service=+ep `readlink -f \`which node\``
```
