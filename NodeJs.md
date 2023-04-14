# How do Webservers Work?

Web servers work by running constantly on the computer, they essentially 'listen' for requests from other computers which are also
connected to the internet.

When they recieve a request, the web server gets the data needed from the storage location, and from the computer which requested it, it will send back this requested
data.

Data can be in text, image, video or other type which will make up a website.

# Node.js & Nginx

* Node.js is a javascript runtime - lets developers run javascript code outside of a browser.

* Use cases are: building webservers, command-line tools, desktop applications

* Node.js has an ecosystem of various 3rd party packages and modules, and developers can use to build their own applications.

# NPM

* Packages are hosted on **NPM**, which stands for node package manager.

* NPM is a tool which is used to install, manage and share packages of code written in Javascript.

* Developers can easily manage what they need to depend on, which are usually external library which their application may
rely on. 

* Developers can use NPM to download install these "dependencies" (refer to ext libraries, modules, packages)
with simple commands.

* NodeJS has different types of dependencies, which showcase the intricacy of its ecosystem. 

* These include: production dependencies, development dependencies, peer dependencies, optional dependencies, 
and bundled dependencies

# Reverse Proxy
 
* It is a server that is usually beteween client devices and webserver.
 
* Clients do not have make requests directly to the webserver, but isntead sent requests to the reverse proxy.
 
* This proxy will then forward the request to the webserver for the client.

