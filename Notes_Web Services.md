
    

- __Microservices__
  : are a variant of Service Oriented Architecture that structures an application as a collection of loosely coupled 
    services. This design brings in modularity and makes the application easier to understand, develop, test and is more resilient to
    architectural corrosion.
    Since the services are independently developed, they can be polyglot in their implementation.
    Also, such a kind of architecture enables continuous delivery and deployment.

    -Microservices vs Serverless
        Serverless also is similar to microservices apart from one thing that in microservice, you need to configure the server
        software and hardware for your service's scalability and operation needs.
        In Serverless, everything is taken care by the third-party provider.


- __Serverless architecture__
  : Serverless architecture also known as Serverless computing or functions as a service is a Software Design Pattern where applications
    are hosted by a third-party service, thus eliminating the need of server software and hardware management by the developer.
    Also, the applications are broken into individual functions that can be invoked and scaled individually.

    Why serverless?
    By adopting the serverless approach, the focus is purely to develop individual functionality in the application code.
    We can say these functions are self-sufficient entities which communicate with other such entities and thus increase 
    the modularity in code.


    FaaS vs SaaS
    Though in SaaS too, you deploy your application on 3rd party servers, but you still need to handle the scalability yourself.
     Whereas 
    In FaaS, each of the functions is autonomous in the sense that it can be scaled up or scaled down as the frequency call increases.
    This actually is a very cost effective approach as you pay only for the time your functions are called.


- __Single Page applications__
    : SPAs are web applications which work on the principle of "load page once and then update thereafter". This eliminates the subsequent
    page reloads because the html file is not sent by the server again. Only the data is sent and it's the responsibility of client to 
    update the html accordingly.
    **** How to go back to previous page if app is Single Page Application.
    Ans:- URL hash technique: e.g. HTML5 History API
    -    Using local hash: Local hash is whatever comes after # in the url. If we change content after #, that wont trigger
    page reload.


- MVC architecture:
    https://developer.mozilla.org/en-US/docs/Web/Apps/Fundamentals/Modern_web_app_architecture/MVC_architecture
    https://msdn.microsoft.com/en-us/magazine/dn463786.aspx
    Is a 3 component architecture commonly used for implementing user interfaces in web apps.
    Model - defines data Structure e.g. updates application to reflect newly added item.
    View - deifnes UI, e.g. user click button to add item
    Controller- contains control logic e.g. receive event from view and then notifies model to take appropriate action eg. add item.

- State Handling for stateless applications(based out of HTTP)
    - Cookies: are client side
    - Sessions: are server side
    - View state/bag: client side



- JSON vs XML:
    • JSON is less verbose than XML because XML needs explicity opening and closing tags
    • JSON has direct mapping for data structures like key-value pairs,strings,arrays in the host language. Although same can be 
        achieved in XML but it would take extra code for serializing and deserializing those data structures.
    • XML requires explicity XML parsers whereas JSON can be parsed using standary JS functions.


- REST
    https://www.mytectra.com/interview-question/api-interview-questions-and-answers/
    Representational State Transfer (REST) is an architectural style that defines a set of constraints to be used for
    creating web services. The client makes a requet asking for a resource identified by URI, to which the server
    takes an appropriate action and sends back the response.
    -REST vs SOAP
        REST is not a protocol. It is an architectural style, whereas SOAP is a protocol. Though REST is not starndard
        but it makes use of standards such as HTTP,JSON,URI,XML.

- Real time web applications
    - Web Sockets: are a protocol which provide a bidirectional channel between the client and the server. This is a different TCP
        protocol than AJAX(HTTP),though both of them reside in layer 7 of OSI.
        Nice explanation: http://blog.teamtreehouse.com/an-introduction-to-websockets
        Web sockets based applications are usually faster because of them being event driven rather than request response/infinite polling. 
        But it has been observed that socket based apps are only 10-20% faster than AJAX based apps.


    - Web Sockets vs REST
        REST is HTTP based(client/server request/response cycle, single direction protocol)
        Web Sockets(Bi-directinal channel where both client and server can send message)

        HTTP requires server polling.
        PUSH notification is core feature of sockets.

        Message Synchronizaton auto handled in HTTP.
        Synchronizaton need to be handled by developer.

        Sockets good for real-time apps such as ongoing football match.

    -You might be using HTTP incorrectly if:

        • Your design relies on a client polling the service often, without the user taking action.
        • Your design requires frequent service calls to send small messages.
        • The client needs to quickly react to a change to a resource, and it cannot predict when the change will occur.
        • The resulting design is cost-prohibitive. Ask yourself: Is a WebSocket solution substantially less effort to design,
        implement, test, and operate?

    -You might be using WebSockets incorrectly if:

        •The connection is used only for a very small number of events, or a very small amount of time,
         and the client does not need to quickly react to the events.
        •Your feature requires multiple WebSockets to be open to the same service at once.
        •Your feature opens a WebSocket, sends messages, then closes it—then repeats the process later.
        •You’re re-implementing a request/response pattern within the messaging layer.
        •The resulting design is cost-prohibitive. Ask yourself: Is a HTTP solution substantially less effort to design,
         implement, test, and operate?


