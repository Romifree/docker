
这是在做低代码平台研究过程中，部署appsmith时碰到的问题。
当时为了把mongo独立出来，花了一个周末在网上查了很多资料，
才终于找到怎么样用docker部署mongo5，并自动配置replica set （appsmith的需求）。
因此共享出来，希望能帮助到类似需求的同学。

It took me a weekend, to deploy mongo5 with auto initializing replica set, which was a must requirement in appsmith.
When I was doing research on lowcode platform and trying to deploy appsmith, 
I could not find a good example and googled a lot before getting it done.
So I'd like to share it with you guys.
1. docker-compose-local-mongo1.yml
    //Single mongo node with replica set
2. docker-compose-local-mongo3.yml
   //Three mongo nodes with replica set
3. docker-compose-remote-mongo3.yml
   //Three mongo nodes with replica set and allow remote connection
4. docker-compose-all.yml
   //Appsmith deployment with separate mongo / redis, and Camunda / pg deployment, which empowers appsmith with workflow feature.