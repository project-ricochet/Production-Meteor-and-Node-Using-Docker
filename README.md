# Production Meteor and Node Using Docker

Thursday, March 17, 2016
Within the field of NetOps, there are many technology channels moving quickly and independently. It’s tricky for a small team to assemble a project using all of the latest technologies in a time frame that won’t crack your spirit.

We’re all constantly assimilating new “buzz” words into our vocabularies. To list a few, there’s Docker, Mesos, Orchestration, DCHQ, ContainerX, Containership, Rancher, Tutum, Continuous Integration, MongoDB replication, mesh networks, Kubernetes (still love the way that sounds), cross cloud deployment, complex DNS, smart load balancing, and...service discovery.

That's a s#!t ton of terms, isn’t it?

I won’t promise Containers will magically make things easier for you. There’s definitely a lot to learn. But just as jQuery helped the sanity of front-end developers, cloud-based Docker services do much the same for NetOps and simplifying Docker deployment.

My mission is to guide you, step by step, through building a production Meteor/Node environment that can deliver a range of cutting-edge application deployment techniques. You’ll be happy to know it’s a very real, robust solution that can scale, works across multiple cloud providers for redundancy, and will help make your business run more smoothly. It will reduce overhead, stress, and perhaps best of all, you can set it all up in a weekend.

Don’t be intimidated. You don’t have to understand everything under the hood to make real progress. Set out to tackle something straightforward on your first attempt. Rest assured — soon you should be able to carefully integrate all the current buzz-wordy technologies that the big guys brag about.

Here’s what I’ll be covering in this post and following posts in the coming weeks:

Why Node and Meteor make great container apps (with example Meteor app and Dockerfile)
Docker Cloud to the rescue (Formerly Tutum.co)
Continuous Integration
Intelligent cross-cloud load balancing (plus Round-robin DNS tricks)
SSL
MongoDB Replication using volumes
Behavioral driven development (BDD)
Backups (not boring anymore!)
Logging and Performance monitoring
If you’re not familiar with Meteor, that should be your first step. It’s well worth getting to know better. Meteor exhibits much the same forward-thinking Docker does. Perhaps that’s why they work so well together.

Node (at the heart of Meteor’s server code) is quite a joy to deploy with Docker. Other languages such as PHP require not only PHP, but a front end web server like Apache or Nginx, plus various modules. Not a “deal breaker” by any means, but Node is dead simple. Don’t you just love simple?

To get comfortable with Docker, it’s important to break down your server needs into small self-contained units (containers!), with each container driving a single process (like Node, or Mongo). In a typical Meteor (or Node) app, your setup will include load balancing, a Mongo replica set (or some other database), and one or more node processes to handle client requests. Here, we’ll outline requirements for a container that will run Meteor/Node. We’ll tackle load balancing and MongoDB in later posts.

#First Two Blogs in Series

_Subscribe or watch for future updates_

[Production Meteor and Node Using Docker, Part I](https://projectricochet.com/blog/production-meteor-and-node-using-docker-part-i#)

[Production Meteor and Node Using Docker, Part II](https://projectricochet.com/blog/production-meteor-and-node-using-docker-part-ii#) 


