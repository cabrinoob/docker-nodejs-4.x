### Utilisation
Dans votre Dockerfile, basez vous sur cette image pour déployer vos applications Node 4.x :

    FROM fmeriot/docker-nodejs-4.x
    
    WORKDIR /nodeapp
    ADD package.json /nodeapp/
    RUN npm install
    ADD . /nodeapp
    
    EXPOSE 80
    CMD []
    ENTRYPOINT ["/nodejs/bin/npm", "start"]
   
   
> Written with [StackEdit](https://stackedit.io/).